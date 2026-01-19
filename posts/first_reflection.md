# Variables and Data tracking

I used multiple variables throughout my code, I used boolean, int, long, float, and PImage. I used long to track the time in my game and control the large numbers returned by the system clock. I needed booleans to manage game states (like the screen stages).

```java
boolean showStartingScreen = true; 
boolean stage1 = true; 
boolean stage2 = true; 
boolean stage3 = true;
float chr_x = 400; 
long startTime; 
long endTime;
```

And I used float to change the values of my character x and character y locations, I used float instead of int so it would be smoother. I used booleans to act like indicators, so my code would switch screens, as an example, if the booleans return false. A problem I encountered when I was coding was that when I was coding my character to jump he wasn’t able to move in the air. The way I fixed this was by adding a key released method, since I originally only had key pressed, and switched my variable type from float to boolean.



