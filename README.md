# Image-Hashing
This image hashing algorithm utilizes image sharpness techniques and ring partition .
The robustness and discriminative power is optimized.

Algorithm :
Binary Hash of Matrix :
1. Take mean of each row and store it in list A
2. Take variance of each row and store it in list B
3. Take skewness of each row and store it in list C
4. Take kurtosis of each row and store it in list D
5. Concatenate list A,list B,list C,list D.
6. Compare each pixel of the final list with its mean, if it's > mean, assign 1 else 0.
7. This final list is the binary hash f the image.

Algorithm for Image Hashing:

1. Convert the image into ring partitions with each ring of equal area
2. Take each ring and combine them to form a matrix with each ring forming 
   a row  of the matrix.
3. Convert the  image to gray scale
4. Resize it to 256*256 pixels
5. Normalize it and pass it through a median filter
6. Return binary hash of the matrix.


Reference papers :

1. https://coek.info/pdf-an-image-sharpening-algorithm-based-on-fuzzy-logic-.html.
2. https://ieeexplore.ieee.org/document/7286814.
3. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5118381/#:~:text=The%20ring%20partitioning%20technique%20converts,generate%20the%20shorter%20hash%20sequence.


