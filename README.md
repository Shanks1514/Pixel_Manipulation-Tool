PIXEL MANIPULATION FOR IMAGE ENCRYPTION

Pixel manipulation for image encryption involves altering the pixel values of an image in a controlled manner to encode secret information or to obscure the original content. 

OBJECTIVES OF THE TOOL

  1 --> Libraries Imported:
        PIL.Image: This module from the Python Imaging Library (PIL) is used for handling image files.
        numpy as np: NumPy is a powerful library for numerical operations in Python. Here, it's used for array manipulation.

  2 --> encrypt_image Function:
        This function takes two arguments: the path to the input image (image_path) and the path to save the encrypted image (output_path).
        It opens the input image using PIL's Image.open() function and converts it into a NumPy array using np.array().
        It performs a pixel manipulation operation (in this case, flipping the image vertically) on the image array using np.flip().
        The resulting manipulated array is converted back to an image using Image.fromarray() and saved to the output image path.

  3 --> decrypt_image Function:
        This function takes two arguments: the path to the encrypted image (encrypted_path) and the path to save the decrypted image (output_path).
        It opens the encrypted image using PIL's Image.open() function and converts it into a NumPy array using np.array().
        It reverses the pixel manipulation operation performed during encryption to obtain the original image array using np.flip().
        The resulting array is converted back to an image using Image.fromarray() and saved to the output image path.

  Example Usage:
        The script defines paths for the input image (input_image_path), the encrypted image (encrypted_image_path), and the decrypted image (decrypted_image_path).
        It calls the encrypt_image() function with the input image path and the output path for the encrypted image. This encrypts the image and saves it.
        Then, it calls the decrypt_image() function with the encrypted image path and the output path for the decrypted image. This decrypts the encrypted image and saves it.

This script provides a basic example of image encryption and decryption using simple pixel manipulation operations.
 
