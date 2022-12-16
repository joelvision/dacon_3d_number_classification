## Dacon Competition
- Link: https://dacon.io/competitions/official/235951/overview/description
- Goal: A competition to classify 3D handwritten numeric images.

## Competition scenario
- At first, we tried to make various attempts based on 3D models.
- However, it was judged that there was a limit to the performance of the 3D model, and to solve this problem, **the existing 3D image was converted into a 2D image through the PCA algorithm.**
- Since the shape is simple and the color is uniform, only efficientnet b0 was used.
- Inspired by the jigsaw puzzle paper, a new augmentation was added.
    - Through this, high level feature extraction was induced. 
    - Above all, performance improved by about 0.3.
- Finally, while learning 50 epochs, a method of excluding or adding specific augmentation was selected for each specific epoch.

## Result
8 / 170