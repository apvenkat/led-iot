Download and Run Code:
Open Raspberry Pi Terminal. If you are doing ssh(remote Access) open Putty and login to raspberry PI.
Create on Directory using following command.


mkdir YourDirectoryName
Go inside that directory using cd command.


cd YourDirectoryName
Then we need git client to download the code from git server.(If you already have git client, skip this step.)

sudo apt-get install git
Download the code using following command.


git clone https://github.com/my-electronics-lab/rpi-led-local-server-nodejs.git

A New directory will be created. Go Inside that directory using cd command.
Inside the project directory, you have to run following command to install all library of node Js. use following command.

npm install
Once all installation will is done, you have to run one more command to start the local server and control the LED.


node index.js
You will see one server message on the console , telling server is started at port 3000.
Now Go to your browser and open raspberry pi URL along with Port Number.which looks something like http://192.168.1.6:3000 (use your Raspberry pi IP)

Enjoy controlling your LED..!!
