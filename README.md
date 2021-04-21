# Idle
An alternative way to keep your computer idle and awake.

#I'm interested in this product. How does it work? 
The idle toolset (Idle.vbs, Idlecheck.bat, and Idlestop.bat) keeps your computer awake by hitting the numlock key twice every 6 seconds. the time interval is configurable as per your desire. it is able to accomplish this in simply 11 lines of code. by hitting the numlock key twice, it returns it to it's original state, but in the process of doing that, it registers a keystroke (2 keystrokes, actually) , which wakes up your computer. 

#I'm sold! How do I get the Idle toolset? 
There are many options. 
- You could download the files from this repository onto a folder on your machine
- You could clone the repository onto your local machine
- You could create these 3 files (Idle.vbs, Idlestop.bat and Idlecheck.bat) onto your machine and re-write the 11 total lines of code that go in these files. should take 2 minutes tops. 

#I have the files on my system. What next? 
- To start the idling process, double click the Idle.vbs file. alternatively, you could click it once and then hit enter. this will launch the script that will keep your computer awake. 

#I ran the Idle.vbs script, but I'm not sure if it worked...
- No problem! If you double click the Idlecheck.bat file, it will run a search for the process that is responsible for idling your machine. if it finds any, you will see "wscript.exe" in the command terminal, which will open upon double clicking the Idlecheck file. if there's multiple "wscript.exe" processes, you may have ran the Idle.vbs file multiple times. it causes no problems to do so. 

#I don't want it hitting numlock every 6 seconds because I'm weird like that. 
- Ok, no problem. simply open the Idle.vbs file in your preferred code editor (Notepad works fine) and put your programmer hat on. You will notice a line of code, specifically one that says "Wscript.Sleep(6000)". the 6000 refers to 6000 milliseconds, which you can change to whichever number you want. after doing so, save the file and exit the editor. re-running the script will create a new process which follows the new rules you just gave it. 

#Alright, I'm ready to stop idling my computer. What can I do? 
- double click the Idlestop.bat file. this will stop all processes labelled "wscript.exe", which is exactly what your Idle process is named. 

Go forth and Idle!
