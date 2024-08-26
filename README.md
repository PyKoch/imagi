# imagiCharms

imagiCharm code features

**Turn the pixel in the first row [0] and the second column [1] on:** 
```
m[0][1] = on
```

**Give the pixel a particular colour, e.g. red:**  
You can choose from: red (R), orange (O), yellow (Y), green (G), aqua (A), blue (B), purple (P), magenta (M), white (W) and black (K).  
This is how you assign the colour: 
```
m[0][1] = R
```

**Assigning RGB colours:**  
Copy and paste the desired colour from your design section on your pixel: 
```
m[0][1] = (242, 5, 0)
```

**Let your pixels blink:**
Pick a blink rate between 0 (not blinking) and 3 (blinking 3 times a second). Floats possible. 
```
m[0][1] = (242, 5, 0)
blink_rate = 1
```
