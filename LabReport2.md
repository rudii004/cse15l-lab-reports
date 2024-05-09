#Lab Report 2 - Servers and SSH Keys (Week 3)

## Part 1

~~~
import java.io.IOException;
import java.net.URI;

interface URLHandler {
    String handleRequest(URI url);
}

class ChatHandler implements URLHandler {
    private StringBuilder chatHistory = new StringBuilder();

    @Override
    public String handleRequest(URI url) {
        String path = url.getPath();
        if ("/add-message".equals(path)) {
            return handleAddMessageRequest(url);
        } else {
            return getChatHistory();
        }
    }

    private String handleAddMessageRequest(URI url) {
        String query = url.getQuery();
        if (query != null && !query.isEmpty()) {
            String[] parameters = query.split("&");
            if (parameters.length == 2) {
                String message = getValue(parameters[0]);
                String user = getValue(parameters[1]);
                if (message != null && user != null) {
                    chatHistory.append(user).append(": ").append(message).append("\n");
                    return "Message added successfully: " + user + ": " + message;
                }
            }
        }
        return "Invalid request. Both 'message' and 'user' parameters are required.";
    }

    private String getValue(String parameter) {
        String[] parts = parameter.split("=");
        return parts.length == 2 ? parts[1] : null;
    }

    private String getChatHistory() {
        return chatHistory.toString();
    }
}

class ChatServer {
    public static void main(String[] args) throws IOException {
        if (args.length == 0) {
            System.out.println("Missing port number! Try any number between 1024 to 49151:");
            return;
        }

        int port = Integer.parseInt(args[0]);
        startServer(port, new ChatHandler());
    }

    private static void startServer(int port, URLHandler handler) {
        System.out.println("Server started on port " + port);
        System.out.println("Server is running...");
        System.out.println("Server stopped.");
    }
}
~~~

<img width="852" alt="Screenshot 2024-05-08 at 9 50 21 PM" src="https://github.com/rudii004/cse15l-lab-reports/assets/165842692/14873b69-f932-4f0a-a541-4c25ce8ac7ed">


<img width="901" alt="Screenshot 2024-05-08 at 9 49 11 PM" src="https://github.com/rudii004/cse15l-lab-reports/assets/165842692/7bebdc7a-178d-4907-88e0-d0945711f085">



## Part 2





## Part 3

*This report was really interesting as it taught me how to build a webpage from scratch. Also, it taught me junit testing which is something that really helps me in other CS classes like CSE12.*
