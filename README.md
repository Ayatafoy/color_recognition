# Color recognition pipeline

##The general algorithm:

- Take image
- Take predicted mask (from segmentation)
- Apply a mask to the image
- Convert each pixel under the mask to LAB color space
- Convert each color to LAB color space
- For each pixel calculate closest pixel from color space using distance metric CIEDE2000 
- Calculate % of each colors from color space having each pixel labeled

Current repo implements this approach using precomputed distances between all RGB pixels and predefined colors 

    

