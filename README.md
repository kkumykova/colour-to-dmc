# Colour to DMC Thread

A CLI tool to translate image colours to closest DMC threads.

To find the colours, the image is quantized and then the nearest colour is looked up from a table of DMC colour threads.

The identified thread numbers will be returned added to the quantized image.

The user can specify the number of colours to reduce the image to before looking up the threads.

The user can also specify the percentage number to use for filtering out the threads as opposed to the default which is set to return all threads used more than 1% in the image.

It's assumed that the user won't be using more than 50 threads to work on. Therefore, if more than 50 threads are returned, only the top 50 most used threads will be added to the output image.

<img src="https://github.com/kkumykova/colour_to_dmc/blob/master/examples/roses_dmc_palette.jpg" data-canonical-src="https://github.com/kkumykova/colour_to_dmc/blob/master/examples/roses_dmc_palette.jpg" width="650" />

# Usage

Tested with Python 3.8.

```
pip install -r requirements.txt
```

