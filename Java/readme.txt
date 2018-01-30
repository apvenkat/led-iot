Here We are going to use Pi4J package for wotking with JAVA

Install Pi4J in yout raspberry pi using the following command given below

curl -s get.pi4j.com | sudo bash        // install Pi4J

After finishing the installation, your Pi4J will be installed in path root/opt/Pi4J

//////////////If installation is unsuccessful, follow below steps////////////////////
Refer, http://pi4j.com/install.html and install the Pi4J 1.2_snapshot version manually because version 1.1 has BCM mismatch error.
//////////////////////  end////////////////////////

After successful installation, Create led_blink.java file in your nano editor using the command
sudo nano led_blink.java          //create java file 

Here I have used GPIO PIN 17 to connect the LED, So make sure you have the same, if you want to connect in different PIN refer below link
http://pi4j.com/pins/model-3b-rev1.html

and chanege in the progam line
final GpioPinDigitalOutput ledPin = gpio.pro
visionDigitalOutputPin(RaspiPin.GPIO_00);           //change GPIO_00 according to your pin number

Java program has to be compiled before executing, So execute the below commands

javac -classpath .:classes:/opt/pi4j/lib/'*' -d . led_blink.java            //compile

Now execute

sudo java -classpath .:classes:/opt/pi4j/lib/'*' led_blink.java      //execute

You should see your led blinking.
