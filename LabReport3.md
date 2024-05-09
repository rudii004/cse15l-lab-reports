# Lab Report 3 - Bugs and Commands (Week 5)

## *Part 1(Bugs)*

Inputs that causes failure

~~~
import static org.junit.Assert.assertArrayEquals;
import org.junit.Test;

public class TestReverseInPlace {
    @Test
    public void testReverseInPlace() {
        int[] input = {10, 20, 30, 40};
        int[] expected = {40, 30, 20, 10};
        
        ArrayExamples.reverseInPlace(input);
        
        assertArrayEquals(expected, input);
    }
}
~~~

Input that does not cause failure

~~~
import static org.junit.Assert.assertArrayEquals;
import org.junit.Test;

public class TestReverseInPlace {
    @Test
    public void testReverseInPlace() {
        int[] input = {7};
        int[] expected = {7};
        
        ArrayExamples.reverseInPlace(input);
        
        assertArrayEquals(expected, input);
    }
}

~~~

## *Symptoms*




*Before fixing bug*

~~~

~~~

*After fixing bug*

~~~

~~~

## *Part 2(Researching commands)*

### *grep -n*
use: This helps us find the lines that have the same phrases
function: it gives the line number for each matching word.

### *Example 1*

~~~

~~~

### *Example 2*

~~~
~~~

### *grep -w*

### *Example 1*

~~~

~~~

### *Example 2*

~~~

~~~

### *grep -c*

### *Example 1*

~~~

~~~

### *Example 2*

~~~

~~~

### *grep -r*

### *Example 1*

~~~

~~~

### *Example 2*

~~~

~~~

## *Sources*






