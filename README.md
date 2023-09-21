Calvin Aduma

This program:
- reads and writes images using OIIO
- converts image 3 channels to 4 channels
- converts RGB to HSV
- green screen masks
- composites an image on top of another


alphamask:
  chmod +x atest.sh
  ./atest.sh

compose:
  chmod +x btest.sh
  ./atest.sh
  
  The program allows you to pick your hue, saturation, and value numbers to test the green screen. You may input values yourself to create your own mask.
