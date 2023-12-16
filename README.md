# PhotoEditor
this is a VERY simple photo editor application that my group is making for their PF proejct. The contributors to this file are: 
1)Fahad Hussain 
2) Ali Roohan 
3) Hasnat 
4)Yaman Tariq

# Main Features
This photo-editor will take ".PNG" files and perform the following filters on them:(grey scale, box-blur, sepia, brightness, Reflection)

# Details

-**Image Manipulation**: The image is implemented in the source file as a 2d- array(row and columns). A PNG image has different sections, the *IMAGEFILEHEADER*, *IMAGEINFOHEADER*, and then the actual bitmap is stored. This is implemented using a Struct in our code that contains all the info about a specific image.

1)**Grey-Scale**: This will take turn a colored image into a black & white image. It takes the RGB values of a single pixle in the image and takes it's average and storing it back. The three colors will cancel each other out when they have the same values, resulting in the final pixel(and then the image) having a color of somewhere between white or black.

2)**Box-Blur**: The image is blured by taking the average RGB values of the neighbours of a certain pixel and then storing them back into it's orignal place. Doing it on the orignal file as it is will cause problems so first we create a copy and store then take the averages using the copy, storing the resultant back into the orignal file.

3)**Sepia**: This is another common filter in most phones. This basically makes the image look "old" just like those captured by cameras that used magnetic tapes. It has many equations but we will be using this one: 

4)**Reflection**: This filter basically flips the image either vertically or horizontally, as per user requirement.

5)**Brigthness**: This changes the brightness of the image by either making it brighter or dimmer. Mathematically, this works by equally increasing the Red Blue and Green values of an image.


# Inspirations and Resources
This whole project takes inspiration from, and then expands upon, Harvard's CS50 problem set 4 "FILTER". The details for that project: https://cs50.harvard.edu/x/2023/psets/4/filter/more/.


