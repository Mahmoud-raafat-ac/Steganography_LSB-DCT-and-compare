![Untitled-4](https://user-images.githubusercontent.com/75928839/118434268-0f8f2880-b6dd-11eb-93b6-a2d7f72f8757.png)
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
