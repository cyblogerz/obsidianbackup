Date: 2024-10-14     Time: 00:34

> [!NOTE]
> Taking notes is  a time consuming process but it will help in making the idea stick . - worth it 
> 
> 

Status: #baby 

Tags : [[flutter]] [[Empowerr]]

# App Lifecycle

![[Pasted image 20241014003618.png]]

# App Lifecycle States in Flutter

1. **resumed**: The app has returned to the foreground and is ready to interact with the user. It transitions from the paused or inactive state.
2. **inactive**: The app is in an inactive state, typically transitioning between foreground and background. User interactions are not processed during this state.
3. **hidden**: The app is in a hidden state, indicating that it is not visible to the user. This state often occurs when the app is minimized or covered by another application.
4. **paused**: The app is paused and not executing code. This state occurs when the app is in the background and not visible to the user.
5. **detached**: The app is completely detached from the framework, indicating that it is about to be terminated.

# Handling life cycle changes in flutter

- `didChangeAppLifecycleState`: This method is called whenever the app transitions between lifecycle states. It receives an `AppLifecycleState`object that indicates the new state. You can use this method to perform actions when the app transitions between states.
-  `dispose`: This method is called when the app is about to be destroyed. You can use this method to clean up any resources that your app is using.


#### Note : Remember to use the `dispose` method to clean up any resources that your app is using when it's about to be destroyed.

### The dispose method

It is called when the widget is permanently removed from the widget tree. 
Quoted from flutter's official documentation :

> [!NOTE]
> 
> The framework calls this method when this [State](https://api.flutter.dev/flutter/widgets/State-class.html) object will never build again. After the framework calls [dispose](https://api.flutter.dev/flutter/widgets/State/dispose.html), the [State](https://api.flutter.dev/flutter/widgets/State-class.html) object is considered unmounted and the [mounted](https://api.flutter.dev/flutter/widgets/State/mounted.html) property is false. It is an error to call [setState](https://api.flutter.dev/flutter/widgets/State/setState.html) at this point. This stage of the lifecycle is terminal: there is no way to remount a [State](https://api.flutter.dev/flutter/widgets/State-class.html) object that has been disposed. Subclasses should override this method to release any resources retained by this object (e.g., stop any active animations).


both initState() and dispose() are part of the widget lifecycle in Flutter. However, they are part of the **Widget’s lifecycle**,


# References
Similar notes and source ideas
[ Medium article about life cycles](https://medium.com/@sharansukesh2000/understanding-flutter-app-lifecycle-a-step-by-step-guide-89676251ac84)
