# Create Prime.java

The fucntion we will write is one that checks if the provided number is a prime or not. Let's create a folder hierarchy for the work:

`mkdir src\main\java`{{execute}}

And enter the java folder:

`cd src\main\java`{{execute}}

Create a java file called Prime.java:

`touch Prime.java`{{execute}}

<pre class="file" data-filename="./cucumber-project/src/main/java/Prime.java" data-target="replace">
package gradle.cucumber;


public class Prime {
    public String play(int number){

        if (number<2) throw new IllegalArgumentException("There are no primenumber less than 2, please provide a larger number");
        for(int i=2; i<number-1; i++){
            if(number % 1==0){
                return "NoPrime";
            }
        }
        return "Prime";
    }
}
</pre>


