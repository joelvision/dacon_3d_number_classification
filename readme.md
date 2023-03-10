## Dacon Competition
- Link: https://dacon.io/competitions/official/235951/overview/description
- Goal: A competition to classify 3D handwritten numeric images.
- Stack: Python, Pytorch  

## Competition scenario
- At first, we tried to make various attempts based on 3D models.
- However, it was judged that there was a limit to the performance of the 3D model, and to solve this problem, **the existing 3D image was converted into a 2D image through the PCA algorithm.**
- Since the shape is simple and the color is uniform, only efficientnet b0 was used.
- Inspired by the jigsaw puzzle paper, a new augmentation was added.
    - Through this, high level feature extraction was induced. 
    - Above all, performance improved by about 0.3.
- Finally, while learning 50 epochs, a method of excluding or adding specific augmentation was selected for each specific epoch.

<img width="554" alt="스크린샷 2022-12-17 시간: 07 15 23" src="https://user-images.githubusercontent.com/118870939/208197853-ca80e5fb-17b6-4118-9db8-759e439f7bf7.png">


## Result
8 / 170
