# Selection Structure

I used selection structure (mostly if statements), to handle collision detection between the character and the platform. This decides whether the character lands on the platform or falls through. 

```java
if (chr_x + 60 > x && chr_x + 20 < x + w) {
 float feetY = chr_y - 80;
    if (feetY >= y - 10 && feetY <= y + 15 && !jumping) {
    onPlatform = true; jumping2 = false; // Stop falling
    chr_y = y + 80; // Snap to top of platform
     }
 }
 ```
I used that code inside of the function createPlatform, the first if statement checks if the character’s x-axis is aligned with the platform's x-axis. Then the inner if statement checks if the player's y-axis is aligned with the platform's y-axis (checking if the player lands on top of it). Also, I added && !jumping so that the character doesn’t go straight to the top of the platform if he’s jumping through the platform. One of the challenges I faced when coding this part was that the character would vibrate on top of the platform. The way I fixed this problem is by adding ```javafeetY >= y - 10 && feetY <= y + 15```, this allows the collision to register even if the character isn’t perfectly aligned.
