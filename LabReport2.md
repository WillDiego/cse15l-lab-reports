# Lab Report Two
1) Server 2) Bugs 3) Summary

## Part 1: String Server
![String Server Code]{StringServerCode.png}
This is a screenshot of the code used to run the server. Areas of note are the two classes Handler and StringServer. StringServer is responsible for running the actual server while Handler is responsible for updating the server by adding new messages.
![Server Running 1]{Server1.png}
* In this screenshot the class being used is the Handler class with the method `handleRequest` being the method doing all of the work.
* The relevant aspects of the method for this specific call is the else statement, in which the code checks the path and if it contains `/add-message`. If it does, which this test does, the code then checks if `s` is included in the first part of the query. Then if it is, the text containing our message is concatinated with the new text with the addition of a new line character. 
* That values that change in this running is just the `String s` at the top of the Handler class. The string is concatinated with the value `"Hello" + '\n'`.
![Server Running 2]{Serever2.png}
* This screenshot is simlar with the class used being Handler class with the method `handleRequest` being the method doing all of the work.
* For this the relevant aspects of the method for this specific call is similar to the last screenshot with the the else statement being used, in which the code checks the path and if it contains `/add-message`. If it does, which this test does, the code then checks if `s` is included in the first part of the query. Then if it is, the text containing our message is concatinated with the new text with the addition of a new line character. 
* That values that change in this running is just the `String s` at the top of the Handler class. The string is concatinated with the value `"Banana!!" + '\n'`.
