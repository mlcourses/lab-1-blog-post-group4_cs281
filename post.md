# Lab 1: Exploring the breadboard and building basic circuits!

## Overview and Motivation
This week's lab introduced us to the breadboard, logic gates and basic circuit components. Through building basic circuits, exploring logic gates and connecting the circuits to different parts of the breadboard, we were able to understamd how the breadboard is configured, how to attach wires to it to build a circuit and how to read circuit diagrams in logic gate specification sheets.

## Materials
1. PB-503 (breadboard)
2. Electrical Wires
3. LED light
4. 330 Ohm Resistor
5. Arduino Kit
6. 7408 AND Gate
7. 7404 NOT Gate

## Part 1: Exploring the breadboard

## Goal
The goal of this part is to understand how to supply power to the breadboard and understand the wiring set-up of the top part of the breadboard.

## Project Steps
To start powering the breadboard, plug the breadboard into a power outlet. Flip on the breadboard switch. If it lights up red, your breadboard is powered!

Now, we explore the structure of the breadboard. The breadboard has two screws at the top right, Red and Black. To start powering the breadboard, do the following. Make sure the breadboard is turned off before doing any wiring!
1. Unscrew the red cap
2. Unscrew the black cap
3. Run a wire under the red cap and connect it to one of the top two rows of the breadboard
4. Run a wire under the black cap and connect it to the one of the bottom two rows of the breadboard.

What we just did was supply 5V to the circuit board with the red pin and then ground the circuit by connecting it to the black (GND) pin.

## Testing
To test the power outputs of each row, plug one end of a wire into any of the rows and the other end into the logic indicator on the right of the breadboard.

When connected to any slots in the first two rows, the logic indicator indicates high. This is because all the slots in the first two rows are connected and the rows are powered by the red (+5V) cap. Similarly, when connected to any slot in the bottom two rows, the logic indicator indicates low.

![Breadboard setup](<IMG_7111 Large.jpeg>){width=250}

The image shows the brown wire coming from a column connected to the +5V power source connected to the logic indicator. The logic indicator shows "HIGH", which is correct.

## Conclusion
After finishing part 1, we know how to connect a power source to the breadboard. We also know how the top of the breadboard is wired and how to test the power output in the breadboard through the use of logic indicators.

## Part 2: Exploring the breadboard (continued)

## Goal
The goal of this part is to explore the wiring setup of the rest of the breadboard.

## Project Steps
Using the previous setup from Part 1, we then do the following steps:
1. Connect a wire from one of the +5V rows to any slot on the lower part of the breadboard
2. Connect a wire from one of the GND rows to another slot on the lower part of the breadboard
3. Connect a wire from the logic input to any part of the breadboard and observe to see whether or not there is signal and whether or not that signal is high or low
4. Move the end on the breadboard to different places on the breadboard to see how the breadboard is wired and which hole is connected to which


## Testing

We noticed there were different sections of the breadboard, a 2-column section and a 5-column section. We also noticed that there were wires connecting the 2-column section to the upper part of the board. We decided to test that first.

We noticed that each column in the 2-column section was connected to the top two rows of the breadboard through either a brown wire or a purple wire. We noticed that the holes in the 2-column section are connected vertically.

When the brown wire is connected to a column connected to the GND row (one of the two lower rows in the upper part of the breadboard), the logic indicator displayed low.

![logic indicator displaying low](<IMG_7113 Large.jpeg>){width=250}

When the brown wire is moved to a column connected to the +5V row (one of the two upper rows in the upper part of the breadboard), the logic indicator displayed high.

![logic indicator displaying high](<IMG_7112 Large.jpeg>){width=250}

We now moved on to testing the 5-column sections. When we first plugged a wire between a hole in the 5-column section and the logic input, we realized that the section had no charge. We realized that we had to connect a wire between either the GND rows or the +5V rows to the breadboard. We connected a red wire between the +5V to the breadboard (notice the left part of the breadboard in the picture above).

We then tested this section of the breadboard. However, when we moved the wire vertically downwards, there was no power in the logic input. We then realized that this section is wired horizontally, meaning the row containing the wire connected to the +5V section all have 5V of power. From this, we also realized that we needed a wire connecting the top part of the breadboard to this section of the breadboard, as there aren’t any wires automatically connected like in the 2-column section.

## Conclusion
After finishing part 2, we nơ understand the set up of the breadboard. To recap, the main part of the breadboard has two types of sections: one with 2 columns and the other with 5 columns. The 2-column section is connected vertically, meaning all holes in the same column have the same charge. The 5-column section is connected horizontally, meaning all holes in the same row has the same charge.

## Part 3: Building a LED-light circuit

## Goal
The goal of this part is to construct a simple circuit on the breadboard that lights up an LED light.


## Project Steps
A complete circuit has to connect +5V to GND. We can add things in between this path, like LED lights or resistors. Therefore, we must first start at a place on the breadboard with a +5V power source. We have two options for this:
1. Use the +5V from the 2-wire section and connect it to a 5-wire section via another wire, giving it power
2. Connect a +5V directly from the upper part of the breadboard to a 5-wire section to give it power

We decided on using Option 1. The next step was to connect the LED light to the circuit. The LED has two legs, a shorter leg and a (slightly) longer leg. Current only flows through then LED one way, with the longer leg connected to the +5V section and the shorter leg connected to the GND section of the circuit. We then connect a resistor from the shorter leg to a GND column in the 2-column section to complete the circuit, connecting the +5V flowing from the source, through the red wire to the longer leg of the LED, then through the shorter leg of the LED, and through the resistor, which leads it to GND. We now have a complete circuit that runs from +5V to GND with attached components (the LED light and the resistor) in between.

## Testing

We followed the project steps outlined above and got the circuit below:

![LED light turned on](<IMG_7115 Large.jpeg>){width=250}

The LED light lights up when we turn the power of the breadboard on! This is because the circuit is complete and so there is power flowing from +5V to GND.

## Conclusion
After finishing part 3, we now understand the requirements of a complete circuit. The circuit has to start at +5V and end at GND and any powered components is in between these two power sources. We now also understand how to wire an LED light, with the longer leg connected to the +5V side of the circuit and the shorter leg connected to GND.

## Part 4: Changing the power source of the circuit

## Goal
The goal of this part is to understand how to change the power source of the circuit, from +5V to a variable power source and to explore about the pulsing power generation capabilities of the breadboard.

## Project Steps
This part will use the same set-up from part 3, with one singular alteration. Instead of connecting the circuit to a +5V power source, we are going to connect it to the function generator on the left side of our breadboard. The function generator generates variable amounts of voltage, which causes the light to “flash”, which is really cool. Because the function generator produces different amounts of voltage, it satisfies the requirement of a complete circuit, which goes from a higher-than-0 voltage source to GND. The completed circuit should look like this:

![Circuit connected to function generator](<connected to function generator.png>){width=250}

## Testing

We messed around with the function generator. Our function generator had a scale that allowed us to change the frequency from 0.1hz to 1hz and then change the units from hz to khz. As we tested, we realized that a larger frequency meant the light was going to flash a lot faster. This is because the frequency of the power source changed how often the power source pulsed voltage through the circuit. Here is a video of us testing the lightbulb at different frequencies:

![](IMG_7119.MOV)

## Conclusion
After finishing part 4, we learnt about the function generator on the breadboard and also realized that the 5V power source is not the only power source that can power the breadboard. We also learnt what frequency meant in terms of electrical pulses.

## Part 5: Hooking Up NOT and AND Gates to the circuit

## Goal
The goal of this part is to understand how to set up the NOT and AND gates in a complete circuit and to learn to test the output of these gates through the use of logic indicators.

## Steps and Testing
We must first look at the data sheet of the NOT gate to see how it is hooked up. The image below shows the top view of the NOT gate:

![not gate specification](<not gate specification.png>){width=250}

According to the specification, the top right leg of the NOT gate is connected to the +5V side of the circuit while the bottom left leg is connected to the GND side of the circuit. After connecting it to the circuit, we must now connect the input and output into the NOT gate. The specification above labels each leg of the NOT gate as either A or Y, with a number in front. A stands for input, while Y stands for output. The number in front “matches” the input and output. For example, a wire coming into 1A will produce an output that can be transferred by a wire coming out of 1Y.

We built the following circuit.

![NOT gate circuit setup](<IMG_7121 Large.jpeg>){width=250}

The circuit is connected to the function generator by the long red wire so the input would change every few seconds from low to high. There is a yellow wire connected to slot 1 on the logic indicator to show the input into the logic indicator. This corresponds to 1A in the specification. According to the specification, the row right below would correspond to 1Y. We connected a yellow wire from a slot in this row to 
slot 2 in the logic indicator. The expected result would be that the logic indicator in slot 2 and slot 1 would always be opposite (one would be high and the other would be low, and vice versa). The result of testing is as follows:

[](<NOT gate circuit testing.MOV>){width=250}

We then looked at the data sheet of the AND gate to see how it is hooked up. The image below shows the top view of the AND gate:

![and gate specification](<and gate specification.png>){width=250}

The setup of the AND gate is not much different from the NOT gate. The top right leg of the AND gate is connected to the +5V side of the circuit while the bottom left leg is connected to the GND side of the circuit. However, instead of having a pair of 1A to 1Y, we have a triplet: 1A, 1B and 1Y. Similar to the NOT gate, the number in front of the letter indicates that the 3 are connected. 1A and 1B are inputs while 1Y is an output. For example, if 1A and 1B are both True (powered by 5V), 1Y will produce HIGH when connected to the logic indicator. If either 1A or 1B is connected to 0V or if both are connected to 0V, 1Y will produce LOW when connected to the the logic indicator.

We tested this by using the logic switches at the bottom of the board. Similar to any other power sources used above (the function generator or the 5V source), there is a wire that runs from the logic switch to the circuit. In this case, two wires are connected to the circuit, one for each input (1A and 1B). We have the following setup.

![and gate setup](<and gate circuit setup Large.jpeg>){width=250}

The image above shows 3 wires connected to the the right side of the AND gate, corresponding to the two outputs (red and purple) and the one output (yellow). The yellow wire is then connected to the logic indicator to show the result of the AND gate. Because the two switches are set to 0, the logic indicator shows LOW. This is correct. We then tried different combinations of input by turning on and off the switches. The video below shows the AND gate working as expected (notice that the light only shows high when both switches are switched up):

![And gate circuit testing](<AND gate circuit testing.MOV>){width=250}

## Part 6: Connecting an Arduino Kit to the circuit

## Goal
The goal of this part is to learn how to connect an Arduino kit to a complete circuit and how basic C coding can be integrated into an electrical circuit.

## Steps and Testing
In this experiment, the Arduino is powered by a USB that is connected to a laptop (the thick blue wire). The USB is also used to transfer data from the laptop to the the Arduino board. For this experiment, we used Arduino IDE to program our Arduino.

![Arduino Code](<Arduino code.png>){width=250}

What this code does is set the Arduino output slot to 13, meaning the output of this code is coming out of pin number 13. This is done through line 6 of the code. The program then sets the power generated by the Arduino to high (line 10), then waits 100 miliseconds (line 11) and then sets the Arduino power output to low (line 12) and then waits 100 miliseconds (line 13). This is then repeated until the Arduino is disconnected or until there is no power source. Note that the time in between High and Low can be changed by changing variables A and B in lines 2 and 3, and the output pin number can be changed by changing variable P in line 1.

The Arduino itself must be inserted into the circuit. Because there is already a power source (from connecting the Arduino board to a laptop), we must also make sure the GND voltage of the Arduino matches that of the circuit. This is done by connecting the GND of the breadboard to the pin labelled GND on the Arduino board. The final Arduino board should look something like this.

![final arduino board]](<final arduno board Large.jpeg>){width=250}

Reusing the AND circuit in Part 5, we have a circuit that looks like the following. The Arduino is connected to Input 1A, while Input 2A is still connected to a logic switch. In the video below, the logic switch is set at 1. The Arduino board is set to pulse high and low, which causes the result from the AND gate to switch from High to Low as well. This is because the input 2A to the AND gate is always 1, while the input 1A (the Arduino board input) loops between 0 and 1.

The video below shows the result of this.

![Arduino testing](<Arduino testing.MOV>){width=250}

We then changed the values of A and B to make change the frequency of the input. By reducing both to 200, we got the following result:

![Arduino changed frequency](<arduino changed frequency.MOV>){width=250}

We also changed P to 7. Before moving the pin, the Arduino stopped working completely. This was because the pin was still on 13, while the Arduino output is now on pin 7. The following video shows that the Arduino works when we rewire from pin 13 to 7.

![Arduino changed pins](<Arduino change pins.MOV>){width=250}

## Conclusion

From today’s lab, we learnt the structure of a breadboard, the setup of a basic circuit, how to read design specifications for gates and how to program and integrate an Arduino into a circuit. The important takeaways are:

1. Breadboards have a 2-column section wired vertically and a 5-column section wired horizontally. They also contain logic indicators, function generators and logic switches, which are used to generate different power supplies for circuits and to test circuit output.
2. A complete circuit is connected from +5V to GND, with components in between.
3. An AND and NOT gate has different rows for inputs and outputs. This can be seen through the design specification of the gates.
4. An Arduino can be programmed to send different electrical signals to the circuit and can be connected directly to the circuit.
