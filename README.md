<h1>Mini Project Slices</h1>

This repository contains small exercises, mini projects, and pieces of larger projects that I either did not finish or concluded were not going anywhere so I saved pieces of them where I learned the most.

<h3>Image Bit Encoding</h3>

I took a large interest in computer science side because I love to know how things work. So I wanted to see if I could "compress" an RGB image. In this little exercise I import an image using Pillow and save its Red-Green-Blue data as a Numpy array, then convert this array into a string of 8-digit numbers (rather than just 9-digit copies of RGB values) to save to a text file as well as a binary file (just to play with). Then I simply re-read in those two files and convert back into the original numpy array to finally display the image once again.

<h3>Multi-Index Pandas Dataframes</h3>

This was part of a very naive project (how embarassing) where I went down a bit of a rabbit-hole into the world of compression. I naively thought maybe you could "compress" very large numbers into much smaller functions. For example the number 26183890704263137277674192438430182020124347 can be "compressed" into 3^91, so I thought maybe you could convert a file's bytes into <b>extremely large</b> numbers and find these "compressible" large-ish numbers within it. Alas though, pigeon-hole theory essentially says this is impossible or at least so extremely unlikely that it'll never work. It may be embarassing to have attempted this, however I did get a lot of practice with Pandas, so I extracted the DataFrame creation in this failed project.
