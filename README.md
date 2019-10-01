# Socket Quiz using Python

This is a socket based multiplayer quiz based on Python

**Instructions**

1. Download the files `server.py` and `client.py`
2. Run this command on your terminal after going into the directory in which the files are stored `python server.py <Your IP Address> <Any Port number>`
3. Open three more terminals(three users) on your desktop and type `python client.py <Your IP address> <Server's port number>` and continue. You could alternatively do this on multiple systems instead of doing this on a single desktop.


**Project Overview**

There are three players in the game. The host (server) has a list of 17 questions and correct answers with him. A question is randomly chosen among the given set of questions and then sends to all the three players. The players press the buzzer by pressing any key on the keyboard. The first one to press the buzzer is given chance to answer the question. If the answer is correct then he is awarded a point, else a negative point awarded. The host then proceeds with the next question. The game stops when the player gets 5 points and then he is declared the winner.


**Project Description**

I have divided the project into two phases, the client phase and the server phase. First the server waits for a connection from the three clients and then proceeds with the questions only if all the three participants have joined. Each of them have been assigned as Player1, Player 2 and Player 3 with respect to the time of their participation. Then the server broadcasts the questions from the stored set of questions in the list given by initiating the clientthread() function. It then waits for buzzer to be pressed from any one of the user and then waits for the user to give some input. If the user gives a correct answer his score is incremented accordingly and reduced if it is a wrong answer.

It keeps on doing the process until a player scores 5 points. And the function end_quiz() is intiated


**Bibliography**

https://www.geeksforgeeks.org/simple-chat-room-using-python/

https://www.youtube.com/watch?v=6jteAOmdsYg&list=PLhTjy8cBISErYuLZUvVOYsR1giva2payF

https://docs.python.org/3/library/socket.html

*Computer Networking: A Top-Down Approach by Kurose and Ross*
