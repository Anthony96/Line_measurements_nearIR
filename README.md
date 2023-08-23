# Line_measurements_nearIR
 Table with measurements of emission lines observed with JWST/NIRSpec in medium resolution mode in CEERS galaxies at redshifts $0<z<3$ selected as described in Calabro et al. (2023) : https://arxiv.org/abs/2306.08605

# Sample description
The CEERS survey and data are presented in Section 2.1 of Calabro et al. (2023), while the sample selection is described in Section 2.1.3 of the same paper. 
In brief, we select those galaxies in which the spectrum covers at least the $H\beta$ + [OIII] triplet and the $Pa\beta$ + [Fe II] triplet. For the final sample, in addition to the two above triplets, we require the identification of the $H\alpha$ + [N II] triplet and the [S III] $9530$ &angst; line, as the presence of all these lines are essential requirements for the analysis of optical and near-IR diagnostics presented in the paper. With these criteria, we have selected 65 galaxies between $z= 1$ and $z= 3$, among which 27 galaxies have $z < 1.75$ and thus also have $Pa\alpha$ detected in the spectrum.

# Emission line measurements
The emission lines are measured with MPFIT (GitHub Repository: stsci.tools/lib/stsci/tools/nmpfit.py, Markwardt et al. 2009) following the procedure explained in Section 2.2 of Calabro et al. (2023). 
We include in the table XXXX.txt the following information for each line :
| suffix | units | description |
| --- | --- | --- |
| _lc | micron | central wavelength of the best-fit gaussian
| _sigma_V | micron | central wavelength of the best-fit gaussian
| _flux | micron | measured flux of the line
| _cont | micron | measured underlying continuum of the line
| _lc | micron | central wavelength of the best-fit gaussian

The $1\sigma$ uncertainties on all parameters are indicated with xxxxx

<hr><hr>
The emission lines fitted are included in the following list : 

| column name | emission line |
| --- | --- |
| CII_1335 | $1335$ &angst; |
| CIV_1551 | $1550.78$ &angst; |
| HeII_1640 | $1640.43$ &angst; |
| CIII_1909 | $1909$ &angst; |
| Hbeta | $H\beta$ |
| OIII_5007 | [OIII] $5006.84$ &angst; |
| Halpha | $H\alpha$ |
| NII_6583 | [NII] $6583.45$ &angst; |
| SIII_9531 | [SIII] $9530.62$ &angst; |
| CI_9850 | [CI]  $9850.26$ &angst; |
| HeI_10830 | HeI $10830$ &angst; |
| PaGamma | $Pa\gamma$ |
| PII_1188 | [PII] $11882.8$ &angst; |
| FeII_1257 | [FeII] $12566.8$ &angst; |
| PaBeta | $Pa\beta$ |
| FeII_132 | [FeII] $13205.5$ &angst; |
| FeII_164 | [FeII] $16435.5$ &angst; |
| PaAlpha | $Pa\alpha$ |
|    |

