# TextureQuilting

TextureQuilting is a student project done in 2017-2018, based on *Image Quilting for Texture Synthesis and Transfer* from Alexei A. Efros and William T. Freeman.

Made by [fonspa](https://github.com/fonspa), [Hyanaki](https://github.com/Hyanaki), [biscotteman](https://github.com/biscotteman) and me.

A short video to explain the process of the algorithm was realized: https://www.youtube.com/watch?v=BAO97-96f84

## Requirements :

- OpenCV version > 3.4

## To build :

```bash

$ git clone https://github.com/nealith/texture-quilting.git
$ cd texture-quilting
$ mkdir build
$ cd build
$ cmake ..
$ make

```

## To use :

Both Texture Synthesis and Generation are executable for testing program. To change parameters, code modification is necessary.

### Texture Synthesis

From a sample image, a texture 1024x1024 is generated.

```bash

$ ./testWeathering <image path>

```

### Texture Generation

Transfer a generated texture from a sample on an element of the image.

To test this program, a function is required as a parameter.
This function is used to create a mask from two images, the input texture and the image containing the object we want to transfer the texture on.
Currently the function is used to transfer a grass texture on the red metal of a ferrari.

## Results

See results folder.
