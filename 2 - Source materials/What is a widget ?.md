
Date: 2024-10-14     Time: 00:48

> [!NOTE]
> Taking notes is  a time consuming process but it will help in making the idea stick . - worth it 
> 
> 

Status: #baby

Tags : [[flutter]]

# What is a widget ?

Widget is a building block in flutter like lego pieces it is somewhat analogous to the components in react js. every thing you see in the flutter app is a widget. They are constructed as a tree - called as the **widget tree** .

### Types of widgets :
- **Stateless widget**  - doesnt have the state
- **Stateful widget**  - has a state


## Stateless widgets
- They doesn't contain states hence inorder to change them , you have to update the parent
- IE, They can only be updated once the parent changes.
- Once created they are immutable , they have to be created again by supplying new data in order to see the changes.

```
import 'package:flutter/material.dart';  
  
void main() => runApp(MyApp());  
  
class MyApp extends StatelessWidget {  
  @override  
  Widget build(BuildContext context) {  
    return Container();  
  }  
}


```

## Stateful widgets

- Can hold states internally , can be updated whenever the state changes as well as whenever the parent changes.
- Its a mutable widget , can be drawn out multiple times in its lifetime.


```
import 'package:flutter/material.dart';  
  
void main() => runApp(MyApp());  
  
class MyApp extends StatefulWidget {  
@override  
_MyAppState createState() => _MyAppState();  
}  
  
class _MyAppState extends State<MyApp> {  
@override  
Widget build(BuildContext context) {  
return Container();  
}  
}

```


![[Pasted image 20241014005858.png]]


## Widget lifecycle methods
- Sequence of events - when a widget is created , updated, or destroyed .

# References
Similar notes and source ideas
[ medium article](https://medium.com/gytworkz/flutter-widget-lifecycle-everything-you-need-to-know-629d01ca4a09)
[[Widget Tree]]