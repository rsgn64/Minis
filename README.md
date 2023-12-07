<h1>Mini Project Slices</h1>

This repository contains small exercises, mini projects, and other pieces of code I wrote to hands-on teach myself certain concepts/libraries. Really just a "hey, I did this" proof of work.

<h3>Image Bit Encoding</h3>

I took a large interest in the computer science side because I love to know how things work. So I wanted to see if I could "compress" an RGB image. In this little exercise I import an image using Pillow and save its Red-Green-Blue data as a Numpy array, then convert this array into a string of 8-digit numbers (rather than just 9-digit copies of RGB values) to save to a text file as well as a binary file (just to play with). Then I simply re-read in those two files and convert back into the original numpy array to finally display the image once again.

<h3>Lucky Compression</h3>

This is now an embarassing project... I naively thought maybe you could "compress" very large numbers into much smaller functions. For example the number 26183890704263137277674192438430182020124347 can be "compressed" into 3^91, so I thought maybe you could convert a file's bytes into <b>extremely large</b> numbers and find these "compressible" large-ish numbers within it. Alas though, pigeon-hole theory and Kolmogorov complexity essentially says this is impossible or at least so extremely unlikely that it'll never work. It may be embarassing to have attempted this, however I did get a lot of practice with Pandas, numpy, mpmath, efficient data storage, etc so I decided to still upload my naivety here, however I did remove the many many lines of playing around with it (way too much text/lines).

<h3>Multi-Index Pandas Dataframes</h3>

This was a mid-way export of a piece of the above project after learning and becoming comfortable with multi-index Pandas DataFrames. I later learned parquet files and other efficient data storage techniques above.

<h3>GPU Compression</h3>

This was an interesting concept I came up with after learning about cost-functions for Machine Learning. I was curious if you could "trade" GPU iterations for file compression since GPU's can do so many iterations so quickly these days.
The concept is to convert a series of x-bytes into integers, use a defined table of numbers to divide them by. If the division results in a whole number AND the resultant number can be stored as 1-byte less than original, record it.
Then attempt to fit these results to some series of functions where the stored info that defines them is less than the total byte reduction + some short-hand indicator that describes the results (such as adding each, or a function that would output a 1 to 2 byte answer.
Afterwards, millions of guessing-iterations can be performed by modern GPUs to decompress.
Ultimately, since my approach isn't quite a cost-function, the concept can't iterate <i>towards</i> the correct answer which I think would make it plausible. This is just guessing and it's a heckin lot of guesses.
