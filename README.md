ASCII Art Donut
This program generates an ASCII art animation of a rotating donut. The animation is created using mathematical formulas to calculate the position and brightness of each pixel in the donut, and printing the pixels to the console using escape codes.

Getting Started
To run the program, make sure you have Python 3 installed on your computer. Then, download the donut.py file and open it in a Python IDE or run it from the command line using the command python donut.py.

How It Works
The program consists of three main parts: functions for calculating sine and cosine, a function for drawing the donut, and a main function that runs the program.

Calculating Sine and Cosine
The calculate_sin and calculate_cos functions use Python's built-in math module to calculate the sine and cosine of an input angle. These functions are used later in the program to calculate the position and brightness of each pixel in the donut.

Drawing the Donut
The draw_donut function generates an ASCII art animation of a rotating donut. The function uses two angles (angle1 and angle2) to calculate the position of each pixel in the donut. It also uses a z_buffer list to keep track of which pixels are closest to the viewer and should be displayed.

The function starts by initializing several variables, including the z_buffer list and a pixels list that will be used to store the ASCII characters for each pixel. It then clears the console using an escape code ("\033[2J") and enters a while loop that will continue until the program is terminated.

Inside the loop, the function clears the pixels and z_buffer lists and calculates the position and brightness of each pixel using a nested for loop. The calculations involve using the sine and cosine functions to manipulate the angles, height, distance, and brightness of each pixel.

After calculating the position and brightness of each pixel, the function prints the pixels list to the console using escape codes ("\033[H" and sys.stdout.flush()). Finally, the function updates the angle1 and angle2 variables for the next iteration of the loop.

Running the Program
The main function simply calls the draw_donut function, which generates the ASCII art animation. The if __name__ == "__main__" line ensures that the main function is only called if the program is run directly (as opposed to being imported as a module).

Contributing
If you have any suggestions for improving the program or finding bugs, please submit an issue or pull request on the GitHub repository.

License
This program is licensed under the MIT License. See the LICENSE file for more details.

Acknowledgements
This program is based on a similar program by Andy Sloane, which can be found here. Thanks to Andy for the inspiration!

Note: This program currently generates multiple donuts instead of just one rotating donut, and the code could use improvement in this regard. Additionally, if you would like to change the resolution of the donut, the relevant code can be found in the draw_donut function, where the variables X and Y are set to control the width and height of the donut.