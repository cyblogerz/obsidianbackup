Date: 2024-10-17     Time: 16:34

*Author: Pranav jay*

> [!NOTE]
> Taking notes is  a time consuming process but it will help in making the idea stick . - worth it 
> 
> 

Status:

Tags: [[flutter]]

# Debouncing
- Debouncing is a programming technique in Flutter - that limits how often a function is called.
- Irps in avoiding performance issues and improving user experience.

Debouncing example :

![[1*S2HFXOuKGbsUqYcbeA1nAw.gif]]


> [!NOTE] From the image
> We can see that the snack bar keeps on showing even after a long time that we clicked. The snack bar persists even if we change the screen. If we clicked continuously, showSnackbar is sent to the event loop and they are executed no matter what. It is working as intended but it leads to a bad user experience. We want to make it so that only the last snack bar is shown leading to a better user experience.


Here it is a snack bar - what if it was an API call? the api would have been called many times. 

##### What is our aim here? - We want to ensure that if an action is performed one after another in a short interval, the previous action is cancelled, and only the latest action is executed. (in this case, tapping a button and showing a snack bar)

###### Debouncing is a technique for preventing unnecessary processing. It involves setting a delay before executing a function so that if the function is called again within the delay, the previous function is cancelled, and the timer is reset again. The function is only executed once the delay has been completed without new events occurring. 


# References
Similar notes and source ideas
[Medium article about debouncing](https://medium.com/codingmountain-blog/debouncing-in-flutter-ed74847e17ff)




