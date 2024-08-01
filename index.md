# Lie Detector Project
Replace this text with a brief description (2-3 sentences) of your project. This description should draw the reader in and make them interested in what you've built. You can include what the biggest challenges, takeaways, and triumphs from completing the project were. As you complete your portfolio, remember your audience is less familiar than you are with all that your project entails!

You should comment out all portions of your portfolio that you have not completed yet, as well as any instructions:
```HTML 
<!--- This is an HTML comment in Markdown -->
<!--- Anything between these symbols will not render on the published site -->
```

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Henry Y | Sage Hill | Mechanical Engineering | Incoming Sophomore

**Replace the BlueStamp logo below with an image of yourself and your completed project. Follow the guide [here](https://tomcam.github.io/least-github-pages/adding-images-github-pages-site.html) if you need help.**

![Headstone Image](logo.svg)
  
# Final Milestone

**Don't forget to replace the text below with the embedding for your milestone video. Go to Youtube, click Share -> Embed, and copy and paste the code to replace what's below.**

<iframe width="560" height="315" src="https://www.youtube.com/embed/F7M7imOVGug" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

For your final milestone, explain the outcome of your project. Key details to include are:
- What you've accomplished since your previous milestone
- What your biggest challenges and triumphs were at BSE
- A summary of key topics you learned about
- What you hope to learn in the future after everything you've learned at BSE



# Second Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/Q7CZFGnQ5iE?si=k9j5a3OE7kBv_rPC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

I have done a lot towards the completion of my project, which is the lie detector. The main work I have done so far is on the technical development of my project. I added a potentiometer in the system so I could adjust and vary the values of resistors. This brings more flexibility and finer adjustment to the circuit, so it's more sensitive, and thus able to respond to variations in skin resistance. Adding three LEDs, namely green, yellow, and red, was also done to show the indication of voltage values when they increase. These LEDs provide instant, clear indication of possible lies: green if the levels are normal, yellow if they are at a moderate increase, and red if they are at a high increase in voltage. I have also changed the code to support these new features so that the LEDs light accordingly, based on the voltage readings. What has really surprised me about this project is the amount of progress I have made and new techniques that I have tried. I never expected to learn and implement all that in such a short time. It was very rewarding to add new components like the potentiometer and LEDs, making them run together. But more engaging was observing changes in the circuit and its code and their impact on the final functional working and accuracy of the lie detector.

One major challenge that I overcame was adding in the potentiometer. The potentiometer used was a 10k one while the old resistor I was using was 1MΩ. This disparity caused the voltage values to always be very low and hard to get proper readings initially. This meant that I had to tune the circuit and the code to work with these now lower values that this 10k potentiometer was giving, which took some trial and error. By defeating this obstacle, I've learned the importance of matching values of components together and the need for tuning in a circuit for optimal performance. There are a few remaining tasks before my final milestone is complete. I will start by adding a heart rate or pulse measurement method so that there could be another signal showing stress or lying. This shall include integrating a heart rate sensor into the existing circuit and updating the code to read and process heart rate data. Second, I will create a house or case for the project to improve the look of the wiring by making sure all of the wiring is hidden, much neater. In so doing, it will give the lie detector professional looks that an end user would want. I will also go back and refine the code and fine-tune the sensors so the lie detector can be as correct and reliable as possible.

# First Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/AADOw3bXJUM?si=9ewBvpXHIUCiqQOu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For my first milestone, I completed the base construction of a machine and some straps for the fingers showing how changes in resistance in my skin will increase the voltage read and printed by the Arduino. The setup uses a voltage divider circuit wherein the higher the resistance, the more voltage absorbed by the resistor. I wired it all together, using an Arduino UNO R3 to be the brain of the project that would process this data and spit out an output. Additionally, I used a breadboard to straighten everything out and to keep all the components in their correct places, and two finger straps made of Velcro and aluminum foil, connected to the fingers in order to get readings of skin resistance. 1 Megaohm (1MΩ) Resistor was used and crucial for the voltage divider circuit, as it provides the ability to measure skin resistance accurately. The 1MΩ resistor is then put in series with the skin resistance being measured through the finger straps. One end of this setup goes to the 5V pin on the Arduino, and the other to an analog input pin, A0. The midpoint, between the resistor and skin resistance, goes to ground (GND). 

During the course of the project, I used a variety of resistor values and had to find the perfect one. I recorded the lowest voltage readings when using resistors of values of lower resistance. This is because it allows more current to flow through them; hence, there will be a lower voltage drop across the resistor. The readings were the highest when I used the 1MΩ resistor. This could be because the higher the resistance, the more it restricts current flow, hence the larger the voltage drop across the resistor. It is the 1MΩ resistor that gave the maximum values obtained so far, hence being the most appropriate for detecting changes in skin resistance. Again, with higher voltage values, I easily noticed changes since these values were more accurate. The higher voltage values gave a finer line of demarcation between the different ranges of skin resistance and thus facilitated the correct detection of a stress response that might indicate lying. In the future I plan to use LEDs to indicate wether the person in fingerstraps if lying or not.

# Schematics 
Here's where you'll put images of your schematics. [Tinkercad](https://www.tinkercad.com/blog/official-guide-to-tinkercad-circuits) and [Fritzing](https://fritzing.org/learning/) are both great resoruces to create professional schematic diagrams, though BSE recommends Tinkercad becuase it can be done easily and for free in the browser. 

# Code
Here's where you'll put your code. The syntax below places it into a block of code. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize it to your project needs. 

```c++
void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  Serial.println("Hello World!");
}

void loop() {
  // put your main code here, to run repeatedly:

}
```

# Bill of Materials
Here's where you'll list the parts in your project. To add more rows, just copy and paste the example rows below.
Don't forget to place the link of where to buy each component inside the quotation marks in the corresponding row after href =. Follow the guide [here]([url](https://www.markdownguide.org/extended-syntax/)) to learn how to customize this to your project needs. 

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |
| Item Name | What the item is used for | $Price | <a href="https://www.amazon.com/Arduino-A000066-ARDUINO-UNO-R3/dp/B008GRTSV6/"> Link </a> |

# Other Resources/Examples
One of the best parts about Github is that you can view how other people set up their own work. Here are some past BSE portfolios that are awesome examples. You can view how they set up their portfolio, and you can view their index.md files to understand how they implemented different portfolio components.
- [Example 1](https://trashytuber.github.io/YimingJiaBlueStamp/)
- [Example 2](https://sviatil0.github.io/Sviatoslav_BSE/)
- [Example 3](https://arneshkumar.github.io/arneshbluestamp/)

To watch the BSE tutorial on how to create a portfolio, click here.
