# KeyboardAssistant
A global keyboard assistant ('global' as in works on every application that runs on the computer).
The project is a keyboard assistant (makes auto-corrections and automatic completion of words), which works on every application that runs on the computer because I worked with a keyboard filter driver which collects the input right from the keyboard itself and can also send data(button clicks) to the computer in the name of the keybord.
My project contains two components frontend(application) and backend which communicate through a socket and deliver data using jsons.
Frontend: the frontend is an application developed using C# Windows Forms App and is very basic, just a small window with three buttons to represent the correction options and three other buttons to represent completion options (which is updated after pressing the update button and requesting the options from the backend)
Backend: a filter driver written in C++ collects hooks from the keyboard and saves the last word and the current one he is trying to write, then it saves the written words to a file, using this information and a basic algorithm the code finds the best 3 corrections\completions (according to the writing status of the user) to offer.
*This project was developed by me and another friend as our final project in our third year in the Magshimim project at the 12'th grade.
