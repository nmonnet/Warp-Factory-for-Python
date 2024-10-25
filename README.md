# Warp factory for Python (analytical approach)
This code reflects my effort to reproduce the results and methodology presented in arXiv:2404.03095, albeit with some modifications. During the process, I identified numerous errors in both their paper and the accompanying code, as well as discrepancies between the two, particularly in the explanations of their examples. Consequently, I chose not to rely heavily on their work to validate my results.

In contrast to their approach, I aim to fully utilize the symbolic capabilities of SymPy and EinsteinPy to derive analytical expressions for the Einstein and Energy-momentum tensors. By minimizing dependence on numerical approximations, this method provides greater precision and flexibility in theoretical analyses at the cost of time. Therefore no numerical approximation are required to obtain the results.

However, the program requires an analytical expression for the inputed metric and more complexe metric defined numerically are impossible to analyze unless you find a good analytical expression for them. Furthermore, the complexity of the analytical expression may radically extend the computation time.

This program will be used to verify the future code of "Warp factory for Python (numerical approach)"
