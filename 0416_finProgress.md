# April 16, 2023 - Final Project Progress Update

I am collaborating with Grace for the final project. We plan to create an interactive sculpture where users place familiar objects on a surface, triggering looping sounds to create a sound collage.

Grace has been painting the objects a single color, making a monochromatic assemblage to be placed on the wall. The idea is for users to pick objects off the wall and place them on their corresponding spots on the surface. We are thinking to create outlines of the objects on the surface, which will probably be a rug, to signify where they're supposed to go. Since we are most likely using magnetically activated reed switches, it won't entirely matter where the users place the objects. While this isn't entirely ideal, it will work for this first version of the project.

As Grace works on the development of the objects and surface, I have been sampling 45's of playful children's music to source some sounds. When that runs out, I will be moving to the BBC sound library and YouTube for more.

## Working on the code

To familiarize myself with working with reed switches, I returned to the button tutorial from Lab 3. I rebuilt the breadboard using two buttons to toggle an LED, then modified the code to work with a single button. Once I had that working, I swapped the remaining button for a reed switch, which I was successfully able to use to toggle an LED based on wether it was activated by a magnet. Being that Grace and I intend on having looping sounds activated by the continued presence of an object, this was a solid step forward.

Next, I started looking at the two p5js sound templates Rob uploaded to the [FSU Digital Media Github page](https://github.com/FSUdigitalmedia) as a jumping off point. I modified the [click2playsound project](https://github.com/FSUdigitalmedia/p5js_click2playsound) to play different sounds based on wether I pressed the left/right arrow keys.

Moving to the [playsound_via_webserial project](https://github.com/FSUdigitalmedia/p5js_playsound_via_webserial), I tried to determine how the Arduino was being used to generate ASCII data which the p5js sketch was using to decide which sounds to play. Since this project constantly creates random data, I wanted to modify the Arduino code to read data from roughly 5-10 switches and generate ASCII values from those.
