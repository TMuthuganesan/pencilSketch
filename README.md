# pencilSketch
It is simple code which uses python openCV library to generate a pencil sketch
from a photo. The steps followed are,
1. Read the input image as gray scale image
2. Remove any noise using a 3x3 gaussian filter
3. Create a negative image
4. Detect the edges from both image & its negative using Sobel
5. Merge these two edge images
    -> These two images reinforces some edges and complements some edges
    -> Alternatively, these two images can be blended with different weights
6. Invert the blended image to get black sketch on white background
7. Show the image and wait for a keystroke to close the display
