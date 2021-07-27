# Simulation 1

This directory consists of csv files of distribution of lenses in the lens plane under a $z_S = 2$ constraint. The visual image can be viewed by running the following command
```
# Create PIL image
img = Image.fromarray(np.uint8(np.transpose(arr_lens_plane_pos[49]) * 255) , 'L')
img.show()
```
It should be noted that the scales are not equal for different images, and more importantly, the pixel_length_x:pixel_length_y $\neq$ 1:1 (It is about 100:1, i.e., the image is disproportionately stretched in the y-direction)
