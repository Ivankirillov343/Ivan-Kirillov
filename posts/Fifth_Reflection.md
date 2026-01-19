# Repetition structure

I used a for loop to generate the platforms for each stage.
```java
for (int i = 0; i < numPlatforms; i++) {
  createPlatform(platX[i], platY[i], platW, platH);
}
```
I used the loop inside ```startGame()```, instead of writing createPlatform multiple times I had a for loop go through the array of coordinates, so that it would then create multiple different platforms. This makes my code more efficient and neat. A challenge I encountered was that I struggled to match the X values with their proper Y values, to fix this I implemented an array and used the index i to match the pairs together.
