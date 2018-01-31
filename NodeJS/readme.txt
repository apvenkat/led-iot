First we will update and upgrade our pi. Run

sudo apt-get update -y && sudo apt-get upgrade -y

This will take quite some time, if you are running this for the first time. (~ 1 hour)

Next, we will download the latest version of Node-ARM

wget http://node-arm.herokuapp.com/node_latest_armhf.deb

Install it by running

sudo dpkg -i node_latest_armhf.deb

If everything works fine without issues, you can run

node -v

and you should see the installed Node’s version.

Here we use onoff Module for our testing, So install the onoff module by running the command

npm install onoff           

Now you can see the node_modules folder having onoff module inside, Now download the led.js file in the same folder and execute the file using the command

sudo node led.js                 // LED will start blinking

