# Arrays and Data Structures

I used arrays to store the x and y coordinates of the platforms for the first, second, and third stage. (code snippet for first stage)
```java
int numPlatforms = 2;
float[] platX = {160, 402};
float[] platY = {400, 400};
```
Where I used it:
```
for (int i = 0; i < numPlatforms; i++) {
    createPlatform(platX[i], platY[i], platW, platH);
  }
```

```platX``` holds the horizontal positions, and ```playY``` holds the vertical positions, for the other stages I have ```platW``` and ```platH``` which are width and height (in stage 1 I have two identical platforms so I didn’t add an array for that). The index 0 would correspond to the first platform and the index 1 would correspond to the second platform. I didn’t encounter any problems with this part.

