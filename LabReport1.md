# Lab Report 1 - Remote Access and FileSystem

*In this lab report we are using the cd, ls and cat commands*

## *cd command*

*Ex 1: cd with No Arguments.*


bash $ cd

<img width="268" alt="Screenshot 2024-04-10 at 6 24 57 PM" src="https://github.com/rudii004/cse15l-lab-reports/assets/165842692/63507931-5d5f-4af9-87c1-275e3828def4">

*Explanation: There is no change in the working directory when you use this command. You are directly taken to your home directory*


$cd /path/to/directory

<img width="365" alt="Screenshot 2024-04-10 at 6 25 09 PM" src="https://github.com/rudii004/cse15l-lab-reports/assets/165842692/68208da3-72e4-43bf-b9a6-1a1efcd86873">

*Explaination: /path/to/directory is now the changed working directory. You can access the directory using ''' cd ''' with a path as an argument*


cd /nonexistent/directory

<img width="328" alt="Screenshot 2024-04-10 at 7 23 38 PM" src="https://github.com/rudii004/cse15l-lab-reports/assets/165842692/12c0e782-a84a-4b7d-82e0-c988837cf722">

*Explanation: The Working directory remains the same as /nonexistent/directory does not exist. Gives an error*


$ ls

<img width="686" alt="Screenshot 2024-04-10 at 6 36 12 PM" src="https://github.com/rudii004/cse15l-lab-reports/assets/165842692/ef8cb3d2-d064-45b9-a46a-f7d592f99633">

*Explaination: This command lists the current files and directories. The output shows the list of all files and directories present*


$ Is /path/to/directory

<img width="399" alt="Screenshot 2024-04-10 at 6 36 35 PM" src="https://github.com/rudii004/cse15l-lab-reports/assets/165842692/1efea8ae-e759-4102-8fc0-698490b4f2d4">


*Explaination: The directory does not change after this command and gives an error.*


$ Is /nonexistent/directory

<img width="327" alt="Screenshot 2024-04-10 at 6 29 08 PM" src="https://github.com/rudii004/cse15l-lab-reports/assets/165842692/96e7e9d3-4bca-43c2-a1f1-0e3db45f6c43">


*Explanation: The working directory does not change again as it does not exist. Gives an error.*


$ cat

<img width="263" alt="Screenshot 2024-04-10 at 6 29 55 PM" src="https://github.com/rudii004/cse15l-lab-reports/assets/165842692/5ea8e86c-1ddb-4f79-a1bb-c0b0df41b11b">

*Explanation: There is no change in the working directory.*


$ cat/path/to/dir

<img width="299" alt="Screenshot 2024-04-10 at 6 37 29 PM" src="https://github.com/rudii004/cse15l-lab-reports/assets/165842692/068207cd-2960-48b0-b372-49b0b726c513">

*Explanation:The working directory remains unchanged.*


$ cat/nonexistent/dir

<img width="322" alt="Screenshot 2024-04-10 at 6 31 55 PM" src="https://github.com/rudii004/cse15l-lab-reports/assets/165842692/c1f50ccc-8758-43f5-b707-46ea4d0b52f9">

*Explanation: The directory does not change as /nonexistent/file.txt does not exist. Gives an error*
