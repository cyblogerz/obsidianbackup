
 Date: 2024-10-14     Time: 19:15

> [!NOTE]
> Taking notes is  a time consuming process but it will help in making the idea stick . - worth it 
> 
> 

Status:

Tags : [[flutter]] [[riverpod]]

# Riverpod + reference architecture

![[flutter-app-architecture.webp]]


## Presentation Layer
- Often called as the UI layer.
- The role of the ui is to act as the primary point of the user interaction.
- The UI is the visual representation of the application state as retrieved from the data layer.

#### The presentation layer consists of two main components
Widgets and controllers.

- ***Widgets*** : representation of the data to be displayed on the screen 
- ***Controllers***:   They perform asynchronous data mutations and manage the widget state. 

```
Presentation layer

Widget -> States -> Controllers

```
###### Note: The controllers themselves are usually represented as [[Asyncnotifier]] sub classes.






# References
Similar notes and source ideas


