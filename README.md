# Welcome to my HTML5 game project's official website.

Below I will be posting periodic updates on progress building this game. I will post short video clips and other information about the latest developments.  

## Update #1
Implemented basic forward and backward movement. I will improve this by adding unique movement mechanics in the future.

![forward_backward](https://user-images.githubusercontent.com/22569153/125556230-15b26343-25dd-4f58-bd36-7db463c46b55.gif)

## Update #2
Implemented turning ability. As mentioned above, a better movement mechanic would drastically improve the gaming experience. Better game mechanics are currently in the `TODO` list in the future. 

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

As you can see below, there are two players using two different browsers (by the way, there can be *more* than just two players). Disregarding where the players are located physically, each player can see each other, move around each other, and share the same world, as long as they are connected to the internet. In other words, the prototype for multiplayer feature is now complete.

![clients_joining](https://user-images.githubusercontent.com/22569153/126854003-5d483857-2b8e-4652-8b0e-ae3bd98cd8d8.gif)



