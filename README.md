# Warp Factory for Python
Warp research has mostly used analytical methods, which often limit the exploration of new solutions. Many proposed solutions have been unrealistic, needing impossible energy levels. To address these issues, people developed Warp Factory (arXiv:2404.03095), a numerical toolkit for modeling warp drive spacetimes. Warp Factory uses numerical analysis to explore various warp drive designs by solving Einstein’s field equations and checking energy requirements. It also offers visualizations in 2D and 3D, helping to understand the metrics and their associated energy structures. Their paper discusses how Warp Factory works and its application in evaluating common warp drive models. Their goal is to advance warp drive research and get closer to creating practical warp drives.

This code represents my efforts to reproduce the results and methodology presented in arXiv:2404.03095, with some modifications. During this process, I identified several errors in both the paper and the accompanying code, as well as discrepancies between the two, particularly in the explanations of their examples. As a result, I chose not to rely heavily on their work to validate my findings.

## Warp Factory for Python (Analytical Approach)
In contrast to the authors' approach, I aim to leverage the symbolic capabilities of SymPy and EinsteinPy to derive analytical expressions for the Einstein and energy-momentum tensors. By minimizing reliance on numerical approximations, this method provides greater precision and flexibility for theoretical analyses, albeit at the cost of increased computation time. As such, no numerical approximations are needed to obtain the results.

However, the program requires an analytical expression for the input metric. More complex metrics defined numerically cannot be analyzed unless a suitable analytical representation is found. Additionally, the complexity of the analytical expression may significantly extend computation time.

This program will also serve to verify the future implementation of the Warp Factory for Python (Numerical Approach).







## Warp Factory for Python (Numerical Approach)
The fully numerical approach employs the simplest numerical approximations to facilitate a direct comparison of its outputs with those obtained from the previous analytical method. Currently, this implementation does not include scalar quantities derived from the metric, and the code related to energy conditions remains largely similar to the earlier analytical approach.

In fact, a purely analytical solution was not feasible, necessitating the use of a semi-numerical approach in the analytical code from the previous section.

At present, the code is not optimized for low-memory systems. To handle high-resolution computations, we are in the process of building a computer with 256 GB of RAM (although 64 GB would typically suffice for standard resolutions). Huge thanks to my friend at TechApart for the PC!



## Information and Disclaimer
Most of the relevant results can be found in the notebook warp_drive_study.ipynb and numerical_warp_drive.ipynb. The older versions containing number in the name are obsolete. In warp_drive_study.ipynb, I strive to explain the differences between my work and arXiv:2404.03095, which is also available as reference_paper.pdf.

This is a passion project that I aim to develop as rigorously as possible; however, I do not have a lot of free time and I do not yet have extensive experience in developing large Python projects, which may affect its overall structure. 

Don't hesitate to leave a comment should you have any questions :) 
