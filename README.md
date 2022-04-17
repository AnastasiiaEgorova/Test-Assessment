# Test-Assessment

Hi there!

I decided to use Boost Asio library for this assessment. I included it as the zip to this project. To be able to use it, it should be included in Additional Include Directories of the solution
(Solution -> Properties -> Configuration Properties -> C/C++ -> General -> Additional Include Directories.) It uses the absolute path, so you may need to change the path to it to run on your machine.

I used a tutorial of how to implement an asyncronous server from here: https://www.boost.org/doc/libs/1_79_0/doc/html/boost_asio/tutorial/tutdaytime6.html

The program works so it waits for sessions to be registered (Director's startup message), then it waits for Actors to send a startup message to be activated in a session. 
(All the Actors' startup messages sent before the Director's startup message are ignored.) Also, it checks for Actors to send a heartbeat message every second; if there is no message, Actor's status is changed to inactive.
The console output provides the information of every session and actors' current statuses. If there is no active session, the console is empty.

Example:
Session: my session
bobspc: inactive
paulsps: inactive
peterspc: active
rachelspc: active

I was able to check it using the Python script you provided.

If you have any questions, please let me know. I will be happy to answer them.

Thanks!
