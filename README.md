# Mathematica_Learning
I want to teach myself Mathematica. All notes are from using Mathematica 11.1.1

## Started with this [tutorial](https://www.youtube.com/watch?v=R4uJMj4TJaQ&list=PLdr5XE6u9kEpS95yKoZwl6kidiFaLnU5s&index=7)

## Shortcuts

```
Alt+7 -> Enter mode 
Ctrl + ( -> Math mode 
Ctrl + _ -> subscript
Ctrl + space -> out of subscript mode 
Ctrl + ^ -> power 
Ctrl + / -> (fractions) and arrow down for denominator
Ctrl + 2 -> square root
Alt + 7 -> type words (not mathematical commands)
Shift + Enter -> Evaluate
Alt + . -> Abort Computation

a2 = N[2, 20] -> 2 means 2 is numerical and 20 is accuracy (ie 20 decimals)

one-based indexing

Length[Listname] -> gives length of list
```

## Plotting Graphs

```
functiontoplot = x + 5 
Plot[function, {x, value, value}, PlotRange->{range1, range2}, PlotStyle->{Thick,Color}]
Two figures overlapping -> Show[Figure1, Figure2]

```

- Plotting by points

```
points = ListPlot [{1,2}, {2,2}, etc]
PlotStyle -> PointSize[.03] where [.03 is size of the point]
```

- Show points after having defined them without displaying 

```
Show[functions, points]
```


## Solving Linear and Simultaneous Equations 

```
Solve[equation == 0, value  to solve for]

= is assignment, so we use ==

Simplify[%] lets Mathematica simplify as best it can

or Expand[%]

Ctrl + / - Fraction and arrow for denominator 

Gives you sets of solutions

FindRoot -> if you display a graph, you can find a precise root 
FindRoot[Var == 0, {x, val}]
```
## Precision

```
WorkingPrecision -> gives to specified number of digits
```

## Loops

```
For loop ->
Define list = {1, 3, 5};
Arr = {};
Do[
	temp = Guess[[k]];
	temp = 2k + k;
	Arr = Append[Arr, temp],
	{k, 1, 3}];
Arr
]

returns {3, 6, 9}
```

- Assumption is that Sin, Cos etc is in Radians

## Questions

- When would I use a Contour/ Implicit Plot
