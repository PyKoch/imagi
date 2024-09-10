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

Now you can modify the code to add the white horizontal line in the middle: 
```
for row in range (0,8):
  if row == 3:
    m[row][col]=W
  else:
    m[row][col]=R
```
