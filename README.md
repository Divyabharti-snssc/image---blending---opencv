# ## Nalanda IT Zone.
* ** Project report under Nalanda it zone internship program.
  # Name : **Divya Bharti
  # Course : **BSC (5th Semester)
  # Session : **(2024-2028)
  # University Roll Number : **(24281200454)
  # University Registration Number : **(24120023228)
  # College Name : **S.N. Sinha College
  
  # Institute Name : **Nalanda It Zone
  
  # Application ID : **(2PFWM0BB)
  
  # Project Topic  : image - blending - opencv

# ## What is Blending ?
* ** In simple terms, **Blending** means mixing to or more different elements together in such a way that the combine into a single uniform entity.
in the world of digital media and image processing blending refres to combining tow different image or video clips seamlessly, so that joint or boundary between them become invisible. this technique is widely used in cinematography for special effects, photo editing 8such as creating double - enposure looks), and graphic designing.

 # What is Image Blending ?
**Image Building** is a fundamental technique in Computer Vision and Digital Image Processing it works By combining the pixel values of two input image based on a specific radio or mathematical formula to generate a new, third image.
this is different from simply placing one image on top of another (overlaying in a simple overly, the top completely hides the bottom one. In blending, ho wever the transparency opacity) of both images is controlled to create a Smooth, translaucent mix.

### Mathematical Formula
\[g(x) = (1-\alpha)f-o(x) + \alphaf-1(x)\]

* ** f0(x):** Background Image
* ** f1(x):** Forground Image
* ** a(Alpha):** Blending factor ranges from '0' to '1')
* ** g(x):** Final Blended Image

# 3. Blending using OpenCV
In OpenCV blending is done using the **'CV2 addWeighted()'** function.

### Rule:
 * Both image must have the **exact same dimensions (weight & height)**  and color channels.

### Python and OpenCV code example:

'''python 
import CV2

# 1. Load both images (Ensure they are located in the same directiory)
image 1. = CV2.imread('image-a.jpg')
image 2. = cv2.imread('image-b.jpg')

# If the image have different size, resize image2 to match image 1:
# image 2. = cv2.resize(image2, (image1.shape[1], image 1.shape[0]))

# 2. Perform blending using cv2. addWeighted()
# Parameters: (src1, Alpha, src2, beta, gamma)
# Hera, Alpha = 0.6(60% weight to image1) and beta = 0.4(40% weight to image2)
final-blend = cv2.addWeighted(image2, 0.6, image2, 0.4, 0)

# 3. Display the final blended image on the screen 
cv2.imshow(Blended output ', final-blend)
# Keep the window open until the user pressea any key
cv2.wait key(0)
cv2.destroyAllWindows()
'''

### Explain of 'cv2.addWeighted()'parameters:

* ** 'srcl' (image1):** The first source image
* ** 'alpha' (0.6):** weight of the first image(determination its opacity/inflaence):
* ** 'scrc' (image2):** The seconds source image
* ** 'beta' (0.4):** Weight of the second image (For optimal results, it is recommended tha 'alpha + beta = 1.0').
*  ** 'gamme'(0):** A scalar value added to each soum. you can use it as a brightness controller for the final output image.


      # Thank You 🌿

        * Thanks to the teacher for guidance and chaking my project file
   

