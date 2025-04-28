# csci111-lab-7-image-processing-solved
**TO GET THIS SOLUTION VISIT:** [CSCI111 Lab 7-Image Processing Solved](https://www.ankitcodinghub.com/product/csci-111-lab-7-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116908&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSCI111 Lab 7-Image Processing Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Image Processing

File names: Names of files, functions, and variables, when specified, must be EXACTLY as specified. This includes simple mistakes such as capitalization.

Image processing: Two dimensional color images are stored on computers in a two dimensional array of colors. A color is a triple of red, green, and blue integer values, each in the range [0,255]. Thus, red is (255,0,0), green is (0, 255, 0), blue is (0, 0, 255) and yellow is (255, 255, 0). Black is (0,0,0) and white is (255, 255, 255).

The PIL module provides functions for loading and storing images on disk in many formats. It also allows you to get and set the color for any pixel. Demonstrations of how to use some of its routines are provided in my demonstration files in the lab folder.

Important: do not use any PIL routines except the ones deonstrated in my code. PIL is a very powerful image processing library and can easily do many of the tasks I’ve set for you below. But you have to do them only with getpixel and setpixel. All the rest is done in Python without PIL routines.

Because we’re going to process images with mathematical functions, it will be much easier to deal with colors as a triple of floating point numbers between 0 and 1. My getpixel and setpixel functions will handle this conversion for you. All computation with colors is done on floats in [0,1], not ints in [0,255]

Provided code: I have provided three modules:

pixel.py Simple utilities for getting/setting pixels and converting from ints in [0,255] to/from floats in [0,1]

separation.py Simple image processing that just extracts the red, green, and blue components of an image.

demo.py A demo program using tkinter that will open an image file and run several image processing algorithms on the image, and show the results in a new window. Simply comment out the parts that aren’t finished until you finish them!

Extract colors: One of the things you can do with an image is just erase two of the three colors. I’ve done this in the separation module, so you can see the effect.

Grayscale: Turning a color image into grayscale is just a matter of adding up all the colors to get a total luminance value for the pixel. Because our eyes are more sensitive to green and red than blue, the sum should be weighted as follows:

gray = 0.299red + 0.587green + 0.114blue

Rather than just taking 1/3 each. You can try both and see which one you like better.

Posterize: Posterizing an image means turning bands of the same luminance into different colors. For example I used black for luminance less than 25%, red for 25% to 50%, magenta for 50% to 75%, and white for 75% to 100%.

Play around with different color bands at different percentages until you get one you like.

Edge detection: Edge detection is a difficult and ongoing field of research. However, a simple algorithm works fairly well. Compute the following quantities for a pixel at (x,y), where L(x,y) is the luminance at (x,y):

The quantity |∇L(x,y)| is the magnitude of the gradient. The larger this value is, the more rapidly the luminance of the image is changing.

If we color only the values of large gradient, we should be coloring the lines. This is just posterizing with white below a threshold and black above.

Hand in: Include my images and code in your lab07 folder, along with your own implementation of the module imageprocessing.py including routines

• grayscale

• posterize (your colors don’t have to match mine)

• edge_detect

Also include an image of your own! I’d prefer your face, but the choice is yours.

Make sure your module works with my demo program! You should not have to change anything in demo.py

Bonus: One bonus lab point! Do sepia as found here

https://dyclassroom.com/image-processing-project/ how-to-convert-a-color-image-into-sepia-image

Remember that our colors have been converted from integers in [0,255] to floats in [0,1]. Do your processing with the floats.
