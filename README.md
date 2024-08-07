<p align="center">
<img width="600" alt="188303830-aa7b11d0-c6ff-4d1a-9bd8-2ccbf4d7e2dd" src="https://github.com/nAuTahn/Mixed-Integer-Optimization-Comparison/blob/main/plot_compare.png">
</p>

# CMA-ES and its problem

$$ f(x) = x_0^2 + x_1^2 \text{ , where } x_0 \in \mathbb{R}, x_1 \in \mathbb{Z} \text{.} $$

|CMA-ES|CMA-ESwM|
|---|---|
|![CMA-ES](fig/CMA-ES.gif)|![CMA-ESwM](fig/CMA-ESwM.gif)|

# Comparison
DX-NES-ICI and LMI-NES (proposed).

## ReversedEllipsoidInt
$$g(x)=\sum_{j=1}^{N_\text{int}}(1000^{\frac{j-1}{N-1}}\left[\bar{\textbf{x}}_{\text{int}}\right]_j)^2$$

$$h(x)=\sum_{j=1}^{N_{\text{co}}}(1000^{\frac{N_{\text{int}}+j-1}{N-1}}[\bar{\textbf{x}}_{\text{co}}]_j)^2$$

$$f(x)=g(x)+h(x)$$

|DX-NES-ICI|LMI-NES|
|---|---|
|![DX-NES-ICI](fig/paperDX-NES-ICI_reversed_ellipsoid_int.gif)|![LMI-NES](fig/LMI-NES_reversed_ellipsoid_int.gif)|

# Reference
1. Ryoki Hamano, Shota Saito, Masahiro Nomura, and Shinichi Shirakawa. 2022. CMA-ES with Margin: Lower-Bounding Marginal Probability for Mixed-Integer Black-Box Optimization. In Proceedings of the Genetic and Evolutionary Computation Conference (GECCO ’22). 639–647. https://doi.org/10.1145/3512290.3528827
2. Koki Ikeda and Isao Ono. 2023. Natural Evolution Strategy for Mixed-Integer Black-Box Optimization. In Proceedings of the Genetic and Evolutionary Computation Conference (GECCO ’23). 8 pages. https://doi.org/10.1145/3583131.3590518
