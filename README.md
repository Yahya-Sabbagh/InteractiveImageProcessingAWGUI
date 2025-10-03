# Image Processing Application

This project is an image processing application that enables users to open images, apply various processing algorithms, and save the results. The application features a responsive graphical user interface (GUI) designed to provide a fluent and smooth experience even during complex image processing operations.

## Features

- **Open Image:**  
  `open_image(file_path)`  
  Opens and displays an image file in the application.

- **Apply Algorithm:**  
  `apply_algorithm(algorithm_name)`  
  Allows users to select and apply a range of image processing algorithms to the currently displayed image.

- **Undo / Redo:**  
  `undo_action()` / `redo_action()`  
  Undo or redo the last image processing actions to support flexible experimentation.

- **Save Image:**  
  `save_image(file_path)`  
  Saves the processed image in a selected format. The save button starts disabled to prevent accidental crashes before an image is loaded or processed.

- **Responsive Processing:**  
  `process_image()`  
  Image processing tasks are executed in a separate thread to keep the GUI responsive.

## Image Processing Algorithms

The application includes the following algorithms:

1. **Gaussian Blur**  
   - `gaussian_blur_window(self)`  
     Opens a dialog to set Gaussian Blur parameters.  
   - `apply_gaussian_blur(self, kernel_size)`  
     Applies Gaussian Blur with customizable kernel size. *(Includes a small extra improvement)*

2. **Sobel Edge Detection**  
   - `sobel_edge_detection(self)`  
     Detects edges in the image using the Sobel operator.

3. **Invert Colors**  
   - `invert_colors(self)`  
     Inverts the colors of the image.

4. **Histogram Equalization**  
   - `histogram_equalization(self)`  
     Enhances image contrast with histogram equalization.

5. **Sharpen Image**  
   - `sharpen_image(self)`  
     Sharpens the image for improved detail.

6. **Drawing Effect**  
   - `drawing_effect(self)`  
     Applies a sketch-like, hand-drawn effect to the image.

## Notes

- The save button is initially disabled to ensure application stability and to avoid crashes before an image is ready to be saved.
- The application is designed for both usability and performance, making sure users can experiment with image processing without GUI interruptions.

---

Thank you for reading, and sorry for taking your time.  
**SABBAGH Yahya**
