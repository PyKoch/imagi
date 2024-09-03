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
**Functions:**  
Functions start with 'def'. A parameter or several can be handed over.  
The function then needs to be 'called' and an argument needs to be set (here the colour red). 
```
def first_column_colour (colour):
  m[0][0]=colour
  m[0][1]=colour
  m[0][2]=colour
  m[0][3]=colour
  m[0][4]=colour
  m[0][5]=colour
  m[0][6]=colour
  m[0][7]=colour

first_column_colour(R)
```
**Loops: for-loops**  
If you want to run code repeatedly, loops are very useful.  
'for'-loops can run for a set number of times.  
```
for x in range (8):
  m[0][x]=R
```

**Loops: while loops**  
If you want to run code repeatedly, loops are very useful.  
While loops run as long as a condition is true.  

```
x = 0

while x<=7:
  m[0][x]=R
  x+=1
```
'x+=1' adds the number '1' to the current value of x.  

**Nested for-loops**
At times it can be useful to have a loop inside another loop. 
If I want to fill the first six rows of the matrix with yellow dots, I can do this with this very short piece of code: 
```
for col in range (8):
  for row in range (6):
    m[row][col]=Y
```



