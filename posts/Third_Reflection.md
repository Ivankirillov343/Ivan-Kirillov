# Custom Functions and Restrictions

I created custom functions like handleJump(), to improve the movement logic and implement restrictions to prevent the character from jumping twice in the air. 
```java
void handleJump() {
    if (!jumping2) {
         if (jumping) {
            chr_y -= 8; time++;
            if (time >= 17) {
                jumping = false;
            }
        }
    }
 }
 ```
The check ```!jumping2``` acts like a restriction, ```jumping2``` is my variable for falling. So this ensures that the character can not jump if they are currently falling off a ledge. The time variable acts like a restriction too. After 17 frames of upward movement jumping turns into false forcing the character to start falling. One of the problems I encountered when making this was that my character could “fly” if you keep on pressing the up arrow key. The way I fixed this was by adding the restrictions !jumping and ```!jumping2``` in the keyPressed function. This makes the code only allow the character to jump if the character is on the ground not moving up or down.


