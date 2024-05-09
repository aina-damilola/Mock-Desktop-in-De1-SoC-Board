# Mock-Desktop-in-De1-SoC-Board
DICLAIMER: Please do not copy and paste this code as it is not to be used for school projects and other submissions,  .

Final project for ECE243 (computer organization) course at the University of Toronto. 

ASSIGNMENT:
To create a program that properly demonstrated the knowledge we gained throughout the course.
We were given a high degree of freedom to what our end goal would look like and with that we 
created a mock desktop with a basic file system.

**Our Project's Functionalities**

Our Desktop & Text Editor project allows for creating, editing, saving and viewing of text files, 
similar to the Notepad app and a simple file system. The inputs are keyboard and mouse for typing 
and cursor movement, and the output is the VGA display. Our project includes a text editor app that 
allows the user to type anything they want on the keyboard, which are displayed on the screen. 
Users can then save the file, which can then be opened later and viewed again.

HOW TO USE:
To guide the user, a white box appears over the selected item when using Keyboard. You can use 
the mouse or the keyboard (arrow_keys and enter key) to navigate most of the selections

*Opening Text Editor and Writing a new text file:*
Click on the text editor app in the task bar or select the app by pressing the down arrow key 
and then Enter. The text editor should show up on the screen. The program now allows typing 
in the text editor. Start typing and keyboard input will be captured and displayed in the text editor.

*In Text-editor:*
Pressing the up arrow disables typing and takes the user to the text editor buttons
There are 3 ways to save a text file:
- Clicking the green button with the mouse or navigating the white box to the green button and clicking enter (the green button is equivalent to “Save”)
- Using the CTRL+S shortcut (Only functional while the selector is not hovering a text editor button i.e red, green or blue)
- Clicking the blue button with the mouse or navigating the white box to the blue button and clicking enter (the blue button is equivalent to “Save as”)

  *Using the Green button* saves the changes made to a file and sets the file name as the first 5characters of the first line as long as the file has not been previously "saved as" 
  *Using the Blue button* sets the name of the file to a maximum of 8 characters, chosen by the user, navigating the “Save” and “Cancel” button by either mouse or using the down arrow     and left right arrow to navigate
  *CTRL+S and ESC* can be used in this window, corresponding to Save and Cancel respectively 

  *Using the Red button* removes any changes from the file and exits the file (if a new file, it doesn't create a file)

*In Desktop:*
Clicking a file brings up the editable file content, displaying the file names at the top bar.
With the arrow keys, you can hover over any file to see the file name at the top of its icon. Pressing enter would open the file.
Hovering over a file and pressing Backspace would delete the file permanently. 
To prevent the outline from ever being stuck, the arrow keys wrap (It moves to the next slot with a file present rather than hovering over an empty slot) 
horizontally while increasing or decreasing in y-level and wrap around vertically only in the upwards direction as the downwards 
direction takes the user straight to the taskbar rather than wrapping around 



**To Demo this Code**

Download the file main.c

Go to https://cpulator.01xz.net/?sys=nios-de1soc  

Change language to c (next to compile and load button)

<img width="435" alt="Screen Shot 2024-05-09 at 1 12 30 PM" src="https://github.com/damilola-aina/Mock-Desktop-in-De1-SoC-Board/assets/163164974/758a83c4-d4f8-443d-8682-15ce7f5efbbb">

Load in main.c

Compile the code and press continue

<img width="218" alt="Screen Shot 2024-05-09 at 1 17 28 PM" src="https://github.com/damilola-aina/Mock-Desktop-in-De1-SoC-Board/assets/163164974/94df7f51-8e49-405a-a796-a2b52b1061f4">

Using the VGA pixel buffer and the PS/2 Keyboard and Mouse, the simulator can mimic the final
project's functionality on the actual hardware. 
NOTE: The y-level of the mouse is reversed online on the simulator as compared to the compiling it on the hardware

<img width="477" alt="Screen Shot 2024-05-09 at 1 13 23 PM" src="https://github.com/damilola-aina/Mock-Desktop-in-De1-SoC-Board/assets/163164974/e040250d-66ec-4701-bf1d-4faed635960a">
<img width="477" alt="Screen Shot 2024-05-09 at 1 13 51 PM" src="https://github.com/damilola-aina/Mock-Desktop-in-De1-SoC-Board/assets/163164974/472a7520-dc52-41a7-873f-394c28b3c724">

Feel free to try it out yourself, If any error arises, here is a video demo taken on the hardware
https://youtu.be/EIrYfBDZ7i8
