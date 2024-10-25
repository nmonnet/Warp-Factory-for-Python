# Warp Factory for Python
This code represents my efforts to reproduce the results and methodology presented in arXiv:2404.03095, with some modifications. During this process, I identified several errors in both the paper and the accompanying code, as well as discrepancies between the two, particularly in the explanations of their examples. As a result, I chose not to rely heavily on their work to validate my findings.

## Warp Factory for Python (Analytical Approach)
In contrast to the authors' approach, I aim to leverage the symbolic capabilities of SymPy and EinsteinPy to derive analytical expressions for the Einstein and energy-momentum tensors. By minimizing reliance on numerical approximations, this method provides greater precision and flexibility for theoretical analyses, albeit at the cost of increased computation time. As such, no numerical approximations are needed to obtain the results.

However, the program requires an analytical expression for the input metric. More complex metrics defined numerically cannot be analyzed unless a suitable analytical representation is found. Additionally, the complexity of the analytical expression may significantly extend computation time.

This program will also serve to verify the future implementation of the Warp Factory for Python (Numerical Approach).

## Warp Factory for Python (Numerical Approach)
My next objective is to translate the original MATLAB code into Python. I will begin with the simplest numerical approximations to facilitate a direct comparison of the outputs with those from the previous analytical approach.

## Information and Disclaimer
Most of the relevant results can be found in the notebook warp_drive_study.ipynb. The older versions are obsolete. In warp_drive_study.ipynb, I strive to explain the differences between my work and arXiv:2404.03095, which is also available as reference_paper.pdf.

This is a passion project that I aim to develop as rigorously as possible; however, I do not have a lot of free time and I do not yet have extensive experience in developing large Python projects, which may affect its overall structure. 

Don't hesitate to leave a comment should you have any questions :) 
