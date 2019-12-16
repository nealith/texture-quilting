# TextureQuilting

A student project done in 2017-2018, based on *Image Quilting for Texture Synthesis and Transfer* from Alexei A. Efros and William T. Freeman.

Made by [fonspa](https://github.com/fonspa), [Hyanaki](https://github.com/Hyanaki), [biscotteman](https://github.com/biscotteman) and me

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

Both of executable are test programm. If you want to change parameters, you have to change de code of each one.

### Texture Synthesis

Generate a 1024x1024 texture from a sample.

```bash

$ ./testWeathering <image path>

```

### Texture Generation

Transfert a gerated texture from a sample on a element in a output image

This test program is more complicated, in fact, the programm need a function as parameter to create transfert mask from the input texture and the output image (the function do the both, since you can test if the input parameter is the texture or the output image )

Currently the function is the function use to transfert a texture of grass on the red metal of a ferarri.

## Results

See results folder.
