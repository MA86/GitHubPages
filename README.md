# Welcome to my HTML5 game project's official website.

Below I will be posting periodic updates on my progress building this game. I will post short video clips and other information about the latest developments.  

My plan is to use various libraries as needed. Up to this point, the languages/libraries that I have used to build this game are the following: 
- JavaScript
- HTML
- Canvas
- Socket.io
- Express
- Matter.js

## Update #1
Implemented basic forward and backward movement. I will improve this further by adding unique movement mechanics in the future.

![forward_backward](https://user-images.githubusercontent.com/22569153/125556230-15b26343-25dd-4f58-bd36-7db463c46b55.gif)

## Update #2
Implemented turning ability. As mentioned above, a better movement mechanic would drastically improve the gaming experience. Better game mechanics are currently in my `TODO` list for the future. 

![rotation](https://user-images.githubusercontent.com/22569153/125557500-10d98679-1fa3-47e4-b5c8-9886950be3ab.gif)

## Update #3
Basic movement is now completely functional.

![move](https://user-images.githubusercontent.com/22569153/125558399-0cdcc371-688f-4b97-8955-2f51d42b7d0a.gif)

## Update #4
Turret can now rotate.

![turr_rot](https://user-images.githubusercontent.com/22569153/125559013-1ec4ebce-9b42-4958-bf55-add9a611a244.gif)

## Update #5
Implemented a basic **server socket** and **client socket** using `Socket.io` library. This is the *first of several steps* needed to add multiplayer functionality to this game project. `Socket.io` library is easy to use and reliable, however it is less efficient for online games with greater than 100 players. 

There are several web networking libraries available to chose from. `WebSocket` library is another option that can be used for TCP messaging.

For online games, using UDP protocol seems to be more recommened because, unlike TCP protocol, UDP does not block if some packets are lost. This will allow for faster multiplayer experience. In the future, I will update to a library that uses UDP.

![socket](https://user-images.githubusercontent.com/22569153/126570785-d0426907-502e-49c8-bed1-35a1f5a50fa9.gif)

## Update #6
Multiple clients can now join and play in the same world from different computers on the internet.

To make this work, I have implemented a server program that all client programs can connect to. My server program is pretty thin, all it does is to sync clients.

As you can see below, there are two players using two different browsers (by the way, there can be *more* than just two players). Disregarding where the players are located physically, each player can see each other, move around each other, and share the same world, as long as they are connected to the internet.

![clients_join](https://user-images.githubusercontent.com/22569153/126854444-6949aa46-2227-42c4-a010-def56f1ba0a3.gif)

## Update #7
When a player leaves the game, every other player knows. 

In the video clip below, player on the right leaves the server. This can be visually seen on the left.

![client_leaves](https://user-images.githubusercontent.com/22569153/127248533-84889e7a-ad28-4f6c-8a07-a829544b5864.gif)

## Update #8
Players are informed when the server crashes. I pressed `Ctrl C` on the server program to simulate server shuting down.

![server_shuts](https://user-images.githubusercontent.com/22569153/127248722-ef60ae27-3edf-4d72-b302-fa330c42f989.gif)

## Update #9
For this update, I used a physics library called `Matter.js` to add physics to this game. It was not an easy task to integrate physics into my existing code, but recently I have been making progress. Unfortunately, I had to break the multiplayer capability for now. Going forward, I will have to figure out a way to add physics for the turret as well. Once this task is complete, I will re-implement multiplayer capability. `Matter.js` provides a powerful and realistic physics, as can be seen in the video below.

![physics](https://user-images.githubusercontent.com/22569153/130541710-415e285a-edd5-4641-bce6-0745782808dd.gif)

