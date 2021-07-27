# Simulation 1

This directory consists of csv files of distribution of lenses in the lens plane under a $z_S = 2$ constraint over a mass range from $1e-16$ to $1e-11$ in equal logarithmic steps `M = np.logspace(-16, -11, 50)` for a radiometric resolution $\epsilon = 0.1$. 
The visual image can be viewed by running the following command
```
# Create PIL image
img = Image.fromarray(np.uint8(np.transpose(arr_lens_plane_pos[k]) * 255) , 'L')    # where k is the image number denoting the mass of the lens
img.show()
```
It should be noted that the scales are not equal for different images, and more importantly, the [pixel_length_x](../pixel_length_x.csv):[pixel_length_y](../pixel_length_y.csv) $\neq$ 1:1 (It ranges from 10:1 to 1e5:1, i.e., the image is disproportionately stretched in the y-direction). 
Images 40 to 49 will give visually recognisable outputs (M ranges from 1e-12 to 1e-11) as the other smaller lenses ideally require better radiometric resolution.
