# Node-Red-Controlled-Neo-Pixel-on-Raspberry-Pi-4

![alt text](https://hackster.imgix.net/uploads/attachments/1628593/_TLfPQ4EyXj.blob?auto=compress%2Cformat&w=900&h=675&fit=min)

NeoPixel LEDs are a popular type of addressable RGB LEDs that can create amazing effects and animations. They are easy to control with a microcontroller like Arduino, but what if you want to use them with a Raspberry Pi? In this article, we’ll show you how to use Node-RED, a graphical programming tool, to control NeoPixel LEDs with a Raspberry Pi.

To follow this tutorial, you’ll need the following components:

A Raspberry Pi board with Raspbian OS installed
A WS2812B NeoPixel LED strip
Some jumper wires
You’ll also need to install Node-RED and the node-red-node-pi-neopixel node on your Raspberry Pi. We’ll explain how to do that later.

![alt text](https://hackster.imgix.net/uploads/attachments/1628595/image_QpUQ1R9evl.png?auto=compress%2Cformat&w=740&h=555&fit=max)

The NeoPixel LED strip has three wires: 5V, GND, and DATA. The 5V and GND wires provide power to the LEDs, while the DATA wire carries the signal that controls the color and brightness of each LED.

The Raspberry Pi can provide 5V and GND from its GPIO pins and connect the DATA pin to GPIO 18. The reason we use GPIO 18 is because it supports PWM (pulse-width modulation), which is needed by the node-red-node-pi-neopixel node. You can use other PWM-enabled GPIO pins, but you’ll need to change the settings accordingly.
Node-RED is a graphical programming tool that lets you create applications by connecting nodes that perform different functions. You can install Node-RED on your Raspberry Pi by following this guide.

To control the NeoPixel LEDs with Node-RED, you need to install a special node called node-red-node-pi-neopixel. This node can drive a strip of NeoPixel or WS2812 LEDs from a Raspberry Pi. You can install it by running the following command.

npm install node-red-node-pi-neopixel
You also need to install the Neopixel python driver, which is used by the node-red-node-pi-neopixel node. The easiest way to do that is to use the Unicorn HAT drivers install script, which you can run with this command:

After installing node-red-node-pi-neopixel, you need to restart Node-RED for the changes to take effect.

![alt text](https://hackster.imgix.net/uploads/attachments/1628598/image_kaKIoFk4iI.png?auto=compress%2Cformat&w=740&h=555&fit=max)

Now that everything is set up, you can create a Node-RED flow to control the NeoPixel LEDs. A flow is a collection of nodes that are connected by wires. Each node has an input and an output and can perform some action or function.

To create a flow, you need to open the Node-RED editor in your web browser. By default, it runs on port 1880 of your Raspberry Pi’s IP address. For example, if your Raspberry Pi’s IP address is 192.168.1.3, you can access the Node-RED editor at http://192.168.1.3:1880.

In the editor, you’ll see a palette of nodes on the left side, a workspace in the middle, and an info panel on the right side. You can drag nodes from the palette to the workspace and connect them by dragging wires from one node’s output to another node’s input.

Here’s an example of a neo-pixel flow that controls the LEDs based on our user inputs.

To create this flow, you need to do the following steps:

Drag Copy and import the below JSON node-red flow.
Change the LED count

![alt text](https://hackster.imgix.net/uploads/attachments/1518136/8_tJuwoRM3dI.JPG?auto=compress%2Cformat&w=740&h=555&fit=max)

You must check out [PCBWAY](https://www.pcbway.com/) for ordering PCBs online for cheap!

You get 10 good-quality PCBs manufactured and shipped to your doorstep for cheap. You will also get a discount on shipping on your first order. Upload your Gerber files onto PCBWAY to get them manufactured with good quality and quick turnaround time. [PCBWay](https://www.pcbway.com/) now could provide a complete product solution, from design to enclosure production. Check out their online Gerber viewer function. With reward points, you can get free stuff from their gift shop.


