# Linear algebra course project Cairo University
![Untitled-4 240x240](https://user-images.githubusercontent.com/75928839/118435111-8d076880-b6de-11eb-9636-2210c197f940.jpg)


# Steganography_LSB-DCT
Steganography Text at images usnig LSB, DCT and compare between them using MSE, PSNR

Standard usage is:

    stego.py [-h] [-d] [-a] -i FILE [-o FILE] [-s STRING] [-f FILE]

```
Stego: DCT and LSB Image Steganography

Optional arguments:
-h, --help  Show this help message and exit
-d          Set method to decode, default is encode
-a          Set encoding/decoding algorithm to LSB, default is DCT
-i FILE     Specify input file name
-o FILE     Specify output file name (optional)
-s STRING   Specify message to encrypt
-f FILE     Specify text file containing message
```

LSB encryption example:

    stego.py -a -i inputFile.png -o outputFile.png -s 'message to encrypt'

DCT encryption example:

    stego.py -i inputFile.png -o outputFile.png -s 'message to encrypt'

LSB decryption example:

    stego.py -a -d -i inputFile.png 

DCT decryption example:

    stego.py -d -i inputFile.png 

## Comparing
   To compare between 2 images
Just go to compare.py and edit the name of images you want to compare.
Then run the code
 
### Python libraries used
•	OpenCV “cv2” (computer vision)

•	Argparse (Parser for command-line options)

•	Pillow “PIL” (Image processing)

•	Numpy (working with arrays)
### Future Work
•	Work with JPG images

•	Work with RGBA images
