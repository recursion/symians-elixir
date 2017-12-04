# SymiansUmbrella

Contains all applications necessary to run a symians server including:
  - Symulator - All the elixir code to create/run/manipulate worlds
  - SymiansServer - The phoenix server - provides an html server and websocker interface to the Syms code
  - Client[X] - Various clients - Currently there is an elm client using SVG display and a typescript client using canvas/phaser for display.
  
  -- Each of these components has its own git repo and must be downloaded and placed into the umbrella/apps folder.
  
  This is a prototype and is in no way complete, but it does currently do some very basic stuff:
  
  Basically the web server calls on the symulator which creates a 3d matrix (the world)and sends a small portion of that data to the client, which displays it. The concept is that the world simulation will run completely independant of the webserver, which only serves to handle connections and pass along relevant data from the simulation.
  
  I really wanted to write the client in elm, but realized early on that I would indeed need to use the html5 canvas element. I started writing a client in typescript with phaser, but just found it incredibly hard to keep using typescript after elm.. and ultimately wandered away from development because of that frustration. i.e. I stopped having fun, which was the whole point. I may pick development back up if I ever find an enjoyable solution for client/canvas development.
