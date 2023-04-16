# Face Recognition 

training the Jetson Nano with individual face images to identify the faces in a group

# Input 
![image](https://user-images.githubusercontent.com/129615197/232349660-b9f0c97d-2d31-45e1-a88a-3f72d996c48f.jpeg)
![image](https://user-images.githubusercontent.com/129615197/232349683-927d5e95-73da-4a30-a5d1-4d2f86715fe2.jpeg)

# Output

![output](https://user-images.githubusercontent.com/129615197/232349894-041830f2-de03-4757-b177-1acf0b682b9e.jpg)

# The Algorithm 

This code is an implementation of face recognition algorithm. Here is the step by step algorithm that this code follows:

1. Import necessary libraries: face_recognition and cv2.
2. Load the known faces (Donald Trump and Nancy Pelosi) and encode them using face_recognition library.
3. Store the encodings and corresponding names in lists.
4. Load an unknown test image and detect the location of faces in the image using face_recognition library.
5. Encode the detected faces in the test image using face_recognition library.
6. Convert the color space of the test image from RGB to BGR (OpenCV format).
7. Loop over the detected faces and compare them with the known face encodings using the face_recognition library.
8. If a match is found, assign the name of the matched person.
9. Draw a rectangle around the face and write the name of the person on the image using cv2 library.
10. Save the output image with the recognized faces and names as "output.jpg" in the current directory using cv2 library.

# Running this project

<img width="907" alt="Screen Shot 2023-04-16 at 5 47 14 PM" src="https://user-images.githubusercontent.com/129615197/232350273-80ae4052-1f4a-48e3-abd6-48773dda49cb.png">

imports cv2 and face_recognition libraries and print the version of cv2

<img width="907" alt="Screen Shot 2023-04-16 at 5 48 44 PM" src="https://user-images.githubusercontent.com/129615197/232350345-6acf3abe-ff6c-4257-a3a3-3390a16c1336.png">

loads two faces, Donald Trump and Nancy Pelosi, encodes them and stores their names and encodings in 2 lists

<img width="907" alt="Screen Shot 2023-04-16 at 5 50 30 PM" src="https://user-images.githubusercontent.com/129615197/232350427-78116905-c9b1-4099-93d8-e99dee941019.png">

This loads a test image, detects the location of faces in the image using face_recognition library, encodes the detected faces, and converts the color space of the image from RGB to BGR (OpenCV format).

<img width="907" alt="Screen Shot 2023-04-16 at 5 51 15 PM" src="https://user-images.githubusercontent.com/129615197/232350486-a3803701-227d-48d0-9e61-b3539eb74a2f.png">

loops over the detected faces, compares them with the known face encodings using the face_recognition library, and if a match is found, assigns the name of the matched person. It then draws a rectangle around the face and writes the name of the person on the image. Finally, it saves the output image with the recognized faces and names as "output.jpg" in the current directory.

# Video Explanation 

