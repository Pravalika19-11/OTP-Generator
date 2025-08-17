# OTP Generator in Java

This project demonstrates a simple **OTP (One-Time Password) generator** program in Java.  
It uses the **Random** class to generate a secure 5-digit OTP.

##  Features
- Generates a random 5-digit OTP
- Uses **anonymous inner class** for method implementation
- Beginner-friendly example of Java abstraction and `Random`

##  Code Example
```java
import java.util.Random;

abstract class MyProject {
    abstract void OTP();
}

class AnonymousRandom {
    public static void main(String[] args) {
        MyProject mp = new MyProject() {
            public void OTP() {
                Random r = new Random();
                int otp = 10000 + r.nextInt(90000); // 5-digit OTP 
                System.out.println("Your OTP is: " + otp);
            }
        };
        mp.OTP();
    }
}
