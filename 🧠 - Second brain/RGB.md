Related topics: [[How to represent information]]

RGB is the way how colors are represented just by setting an amount of red, green and blue, by mixing different amounts of them we can get a lot of colors which we see represented in our screen.

![[RGB.png]]

Indeed our screens work in this manner, our screens aren’t more but a bunch of pixels which at the same time are groups of three lights one red, one green and one blue:

![[Pixels.png]]

Know of a computational way we represent this amount with a byte, we assign a byte for each color, one for the red, one for the green and one for the blue, and the higher that number is the brighter the color is.

So [[images]] are just a extensive bunch of RGB values arranged in a bi-dimensional space. Indeed a video are a sequence of [[images]] changing over the time plus a audio running at the same time.

Now the RGB commonly is represented through the amount of each pixel, for example 0, 0, 0 the color black, and 255, 255, 255, represents the white, all these values are of course stored in [[Binary]] system inside the computer, for example white would be 11111111, 11111111, 11111111. Nevertheless, it is a little hard for humans to understand and tedious to deal with. So to make it easier, we represent them in something similar as this: 

\#ffffff // this represents the same pure white color

Now what we're doing is just putting the three values together but in a [[Hexadecimal]] value.