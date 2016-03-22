data-structures-problem
=======================

Start of the Data Structures toy problem

##Background

Your up-and-coming website, Chat-tastic, is set to bring back the chatrooms like no one's ever seen. We're talking 1999, baby.

There is a "server" component to your website that handles all of the users coming and going. Every so often, a new user will join the website and the server will call a function in the global scope called `new_user_joined`. Periodically, the server will also call a function in the global scope called `assign_to_chatroom` which will give you the ability to proportion users where they need to go.

Your job is to assign the users to chatrooms based on their order of appearance (first come first served). You should also try to keep the chatrooms equally full.

##Objectives

###1. Capture all incoming users in an appropriate data structure in the function `new_user_joined`

Because you don't know when new users will be coming, you need to capture all of them so that when the assign_to_chatroom function is called, you're ready to assign them to an appropriate room.

**Hints**
* Open up the page in your brower and look at the console. The logs coming through should give you an indication of when different methods are being called.
* The `users_joined` array is already provided for you as a start
* Which data structure uses the "first come first served" policy? What are that data structure's methods?
* Use the `new_user_joined` function when you're adding users to your data structure

###2. Assign users in order of appearance to a chatroom
Every five seconds the server will call the function `assign_to_chatroom` and you'll need to place each user in your data structure to a chatroom. A button element (see the commented code in `assign_to_chatroom`) needs to be added for every new user in each room.

**Hints**
* In the `assign_to_chatroom` function, you'll go through your users_joined data structure, pulling out users in order of appearance and inserting them into the DOM via jQuery
* To keep both containers equally full, you could:
  * Create a variable that tells you which container you're going to use next, then when you've used it, point the variable to the other container
  * Create a boolean variable that when true, indicates using one container and when false, indicates you should use the other. Change the boolean every time a student is assigned.

###3. (Black Diamond) Make sure there are no repeats of users in a room

**Hints**
* See the `chatrooms` variable? What data struture does that look like? How could you use it to make sure there are no repeated users?


## Copyright

© DevMountain LLC, 2016. Unauthorized use and/or duplication of this material without express and written permission from DevMountain, LLC is strictly prohibited. Excerpts and links may be used, provided that full and clear credit is given to DevMountain with appropriate and specific direction to the original content.
