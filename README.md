# Ticket-Ordering-Process
In this project I used semaphores and threads to simulate phonecalls to the tonight show. 
Semaphores are declared globally and initialized in the main function. 
A for loop creates how ever many threads or "phonecalls" I want.
In the handler function the thread is given an id from 1 to callercount using a global variable.
A binary semaphore is used to do this to avoid race conditions. 
Then a while loop simulates the repeated effort of calling the show until a call gets a line. 
From there a counting semaphore is used to connect it to the operator and the rest is history. 

