Client:
Receive info from server a. Use it to render the grid
Receive movement from user a. Send it to the server

Server:
All player positions and score a. Send info to client
Receive player movement from client a. Send it to all the clients (1)
Set up position for the grid (player spawn and tomato)
Synchronization to make sure players are not going to the same position
Server sends to each client: (player1.x,player1.y,player2.x,player2.y,player3.x,player3.y,player4.x,player4.y,level,score,NumOfTomatos,playerId)

(After player moves) Each client sends to the server: (playerId.x, playerId.y)