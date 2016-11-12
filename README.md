# PatapClone

This is a Patap clone (http://patatap.com/). It was made purely for learning purposes. The app takes advantage of Paper.js for animations, as well as Howler.js for playing the various sounds. 

As of right now, the app has a dedicated sound for every letter key. If a user clicks on any other key, they will recieve an alert with telling them that there is no sound associated with that key. Also, each key is defined inside a "keyData" JS object that is prased through to determine the start color and sound for the key.


# Paper.Js
Paper.JS takes advantege of HTML's canvas element. Inside the canvas, a onKeyDown() event will trigger the creation of a circle randomly on the screen based on the size of the screen. This is accomplished with Paper.js's view attribute that allows the app to change based on the view size. The current max width, and height are stored in a variable and multiplied by Point.random(). Then a new circle is created and given the random x,y coordinate, color, and sound.

