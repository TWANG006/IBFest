## Introduction
IBFest is the research code for ion beam figuring (IBF) system for synchrotron X-ray mirrors designed and developed by the Optical Metrology and Fabrication Group at National Synchrotron Light Source II (NSLS-II), NY, US. 

## Implemented algorithms
- [x] Rectangular surface error map simulation using 2D Lengendre polynomials
- [x] 2D Beam Removal Function (BRF) fittintg and learning
- Dwell time calculation algorithms
  - Fourier domain methods
    - [x] Fourier transform + Inverse filtering [2]
    - [x] Bayesian iterative method [4]
    - [ ] Robust Iterative Fourier Trasform-based dwell time Algorithm (RIFTA) [8, 9]
  - Matrix-based methods
    - [x] Truncated SVD (TSVD) [3]
    - [x] LSQR [1, 5]
    - [x] Constrained Linear Least Squares (CLLS) + Coarse-to-Fine scheme [6, 7]

## Reference
[1] [Carnal, C. L., Egert, C. M., & Hylton, K. W. (1992, December). Advanced matrix-based algorithm for ion-beam milling of optical components. In Current Developments in Optical Design and Optical Engineering II (Vol. 1752, pp. 54-62). International Society for Optics and Photonics.](https://doi.org/10.1117/12.130719)

[2] [Wilson, S. R., & McNeil, J. R. (1987, January). Neutral ion beam figuring of large optical surfaces. In Current Developments in Optical Engineering II (Vol. 818, pp. 320-324). International Society for Optics and Photonics.](https://doi.org/10.1117/12.978903)

[3] [Zhou, L., Dai, Y. F., Xie, X. H., Jiao, C. J., & Li, S. Y. (2007). Model and method to determine dwell time in ion beam figuring. Nanotechnol. Precis. Eng., 5(8–9), 107-112.](http://en.cnki.com.cn/Article_en/CJFDTotal-NMJM200702009.htm)

[4] [Jiao, C., Li, S., & Xie, X. (2009). Algorithm for ion beam figuring of low-gradient mirrors. Applied Optics, 48(21), 4090-4096.](https://doi.org/10.1364/AO.48.004090)

[5] [Wu, J. F., Lu, Z. W., Zhang, H. X., & Wang, T. S. (2009). Dwell time algorithm in ion beam figuring. Applied optics, 48(20), 3930-3937.](https://doi.org/10.1364/AO.48.003930)

[6] [Wang, T., Huang, L., Vescovi, M., Kuhne, D., Tayabaly, K., Bouet, N., & Idir, M. (2019). Study on an effective one-dimensional ion-beam figuring method. Optics express, 27(11), 15368-15381.](https://doi.org/10.1364/OE.27.015368)

[7] [Wang, T., Huang, L., Vescovi, M., Kuhne, D., Tayabaly, K., Bouet, N., & Idir, M. (2019, September). One-dimensional ion-beam figuring solution from Brookhaven National Laboratory. In Advances in Metrology for X-Ray and EUV Optics VIII (Vol. 11109, p. 1110909). International Society for Optics and Photonics.](https://doi.org/10.1117/12.2526074)

[8] [Wang, T., Huang, L., Tayabaly, K., & Idir, M. (2019, November). Study on the performances of dwell time algorithms in ion beam figuring. In Optifab 2019 (Vol. 11175, p. 111750M). International Society for Optics and Photonics.](https://doi.org/10.1117/12.2536869)

[9] T. Wang, L. Huang, H. Kang, H. Choi, D. W. Kim, K. Tayabaly, andM. Idir, “Rifta: a robust iterative fourier transform-based dwell time algo-rithm for ion beam figuring,” Sci. ReportsUnder peer review(2019)
