# CSCI3202 Introduction to AI
This is the third assignment for the course "Introduction to AI"<br>
The .py program takes two argument. First is the file of the World. Second is the heuristic function.<br>
Now there are two heuristic functions to choose:
* Manhatten distance, by entering Manhatten
* Euclidean distance, by entering Euclid<br>
eg. "python astar.py World1.txt Manhatten"

I used Euclidean distance in the second heuristic.<br>
Equation: square root((node.x-end.x)^2+(node.y-end.y)^2)<br>
Movivation: Because Euclidean Distance is more closer to the reality. In the case of World1 and WWorld2, We start from the left lower corner end at the right higher corner. Euclidean is more closer to the straight distance, and can evaluate the distance to the end more accurately.<br>
Manhatten
---------
In world1:<br>
total cost = 156<br>
location evaluated = 98<br>
path:(7,0)(6,1)(5,1)(4,1)(3,1)(2,2)(2,3)(1,4)(0,5)(0,6)(0,7)(0,8)(0,9)<br>
<br>
In world2:<br>
total cost = 150<br>
location evaluated = 71<br>
path:(7,0)(6,1)(5,0)(4,1)(4,2)(4,3)(3,4)(2,4)(1,4)(0,5)(0,6)(0,7)(0,8)(0,9)<br>

Euclidean
--------
In world1:<br>
total cost = 138<br>
location evaluated = 156<br>
path:(7,0)(6,1)(7,2)(6,3)(5,4)(4,4)(3,5)(3,6)(2,7)(2,8)(1,9)(0,9)<br><br>
In world2:<br>
total cost = 152<br>
location evaluated = 104<br>
path:(7,0)(6,1)(7,2)(6,3)(5,3)(4,4)(3,5)(3,6)(2,7)(1,8)(0,9)<br>

In World1, Compare to using Manhatten distance, using Euclidean distance can get a lower cost path, but more evaluated locations.<br>
In World2, I get the opposite result. The Euclidean heuristic function result in higher cost but less evaluated locations.<br>
In conclusion, neither of the two heuristic functions is better than the other. It depends on the environment.
