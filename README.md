# Welcome to my HTML5 game project's official website.

Below I will be posting periodic updates on progress building this game. I will post short video clips and other information about the latest developments.  

## Update #1
Implemented forward and backward movement.

![forward_backward](https://user-images.githubusercontent.com/22569153/125556230-15b26343-25dd-4f58-bd36-7db463c46b55.gif)

## Update #2
Implemented turning ability.

![rotation](https://user-images.githubusercontent.com/22569153/125557500-10d98679-1fa3-47e4-b5c8-9886950be3ab.gif)

## Update #3
Tank movement is now completely functional.

![move](https://user-images.githubusercontent.com/22569153/125558399-0cdcc371-688f-4b97-8955-2f51d42b7d0a.gif)

## Update #4
Tank turret can now rotate.

![turr_rot](https://user-images.githubusercontent.com/22569153/125559013-1ec4ebce-9b42-4958-bf55-add9a611a244.gif)

## Update #5
Implemented a basic socket server and socket client using `Socket.io` library. This is the first of many steps needed to add multiplayer functionality to this game project. There are several web networking libraries available to chose from. `WebSocket` library is another option that can be used for TCP messaging. `Socket.io` library is easy to use and reliable, however it is less efficient for online games with greater than 100 players.

For online games, using UDP protocol seems to be more recommened, because unlike TCP protocol, UDP does not block if some packets are lost. This will allow for faster multiplayer experience. In the future, will update to a library that uses UDP.

![socket](https://user-images.githubusercontent.com/22569153/126570785-d0426907-502e-49c8-bed1-35a1f5a50fa9.gif)



