## Lesson 10

### Warm-up: 
Write Python code on edu.imagilabs.com that does the following: 

- Uses a function with the parameter 'colour'
- the function should draw a diagonal line (either direction)
- aim for 'Pythonic' code, i.e. very few lines of code
- call the function with a colour of your choice as the argument, e.g. R (red)

### Develop your proficiency of using functions: 
- Try out the background function: 
- Write two functions: one for vertical lines and one for horizontal lines

![640px-Flag_of_Finland svg (1)](https://github.com/user-attachments/assets/a8bc25f3-7d8b-416e-9489-c4d060a35ad8)

By SVG Vectorization: Sebastian Koppehel - https://finlex.fi/fi/laki/ajantasa/1978/19780380 https://finlex.fi/fi/laki/alkup/1993/19930827 https://encycolorpedia.com/002f6c, Public Domain, https://commons.wikimedia.org/w/index.php?curid=343054

### Conditions: using if-statements: 
In Coding conditions allow you to execute code based on specific criteria. 
In Python you generall write: 

```
if ...:
  do this
elif ...:
  do that
else:
  do something else
```

We can use the 'if-statement' in this context e.g. for creating the Austrian flag: 

![640px-Flag_of_Austria svg](https://github.com/user-attachments/assets/444dc35a-2973-4fa0-8be4-62c3846356d6)

By Bundesministerium für Landesverteidigung - Dekorationen, Insignien und Hoheitszeichen in Verbindung mit / in conjunction with Grundsätzliche Bestimmungen über Verwendung des Hoheitszeichens sowie über die Fahnenordnung des Österreichischen Bundesheeres. Erlass vom 14. Mai 2018, GZ S93592/3-MFW/2018., Public Domain, https://commons.wikimedia.org/w/index.php?curid=342954

Say you would initally fill every row with red dots: 

```
for row in range (0,8):
  for col in range (0,8):
    m[row][col]=R
```

<img width="250" alt="red_dots" src="https://github.com/user-attachments/assets/283ea0c2-affa-4fb0-b8a3-21cccf623f3c">

Now you can modify the code to add the white horizontal line in the middle: 
```
for row in range (0,8):
  for col in range (0,8):
    if row == 3:
      m[row][col]=W
    else:
      m[row][col]=R
```
<img width="250" alt="austrian" src="https://github.com/user-attachments/assets/0e801ead-899d-4bd7-b186-2d7bb6a4b96b">

As an Austrian, you might not be satisfied with this result. 
One solution would be to use the elif statement: 

```
for row in range (0,8):
  for col in range (0,8):
    if row == 3:
      m[row][col]=W
    elif row ==4:
      m[row][col]=W
    else:
      m[row][col]=R
```

<img width="260" alt="austrian2" src="https://github.com/user-attachments/assets/f0a1b38c-991e-41dc-a37a-6c22a3c0d98b">

### Challenge: 
Use conditions to draw the German flag: 

<img width="253" alt="German" src="https://github.com/user-attachments/assets/2dc9dfa1-d102-4988-926a-5522c68d7ef8">
