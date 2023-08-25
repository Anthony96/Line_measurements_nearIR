# Line_measurements_nearIR
 Table with measurements of emission lines observed with JWST/NIRSpec in medium resolution mode ($R \simeq 1000$) in CEERS galaxies at redshifts $0 < z < 3$ selected as described in Calabro et al. (2023) : https://arxiv.org/abs/2306.08605

# Sample description
The CEERS survey and data are presented in Section 2.1 of Calabro et al. (2023), while the sample selection is described in Section 2.1.3 of the same paper. 
In brief, we select those galaxies in which the spectrum covers at least the $H\beta$ + [OIII] triplet and the $Pa\beta$ + [Fe II] triplet. For the final sample, in addition to the two above triplets, we require the identification of the $H\alpha$ + [N II] triplet and the [S III] $9530$ &angst; line, as the presence of all these lines are essential requirements for the analysis of optical and near-IR diagnostics presented in the paper. With these criteria, we have selected 65 galaxies between $z= 1$ and $z= 3$, among which 27 galaxies have $z < 1.75$ and $Pa\alpha$ is detected in the spectrum.

# Table with emission line measurements 
The emission lines are measured with MPFIT (Markwardt et al. 2009) following the procedure explained in Section 2.2 of Calabro et al. (2023). 

The spectroscopic redshift z<sub>spec</sub> and the velocity width $\sigma$ of the lines are determined from the highest S/N emission line (typically $H \alpha$ or [SIII] $9530.62$). **These values are then fixed when fitting the remaining lines**, with a tolerance of $500\ km/s$ and $100\ km/s$, respectively. 

#
In this repository we include the table *public_release_line_meas_Calabro23_vers1_optical.txt*, with the main properties of the galaxies in the first three columns :

| column name | units | description |
| --- | --- | --- |
| ID | - | ID of the galaxy in the CEERS MSA catalog
| RA | deg | Right Ascension of the source (this refers to the center of the MSA as observed by CEERS)
| DEC | deg | Declination of the source (this refers to the center of the MSA as observed by CEERS)

then we include for each line the following information :
| column suffix | units | description |
| ---- | --- | --- |
| _flux | $10^{-19}$ $erg/s/cm^2$ | measured flux of the line 
| _flux_err | $10^{-19}$ $erg/s/cm^2$ | $1\sigma$ uncertainty on the flux 
| _cont | $10^{-19}$ $erg/s/cm^2$ | measured underlying continuum of the line 
| _sigma_V | km/s | observed $\sigma$ of the best-fit gaussian of the line (only for $H\beta$, $H\alpha$,[SIII] $9530.62$, HeI $10830$, $Pa\beta$, $Pa\alpha$)
| _redshift | - | redshift estimated from the central wavelength of the best-fit gaussian as</br> [$\lambda$<sub>central</sub>/$\lambda$<sub>line, restframe</sub>-1] (only for $H\beta$, $H\alpha$,</br> [SIII] $9530.62$, HeI $10830$, $Pa\beta$, $Pa\alpha$)

**N.B. If the error value is $-1$ (i.e., _flux_err $=-1$), the flux of the corresponding emission line should be treated as an upper limit.**

<hr><hr>
The emission lines fitted and reported in the table are listed below : 


| column prefix | emission line |
| ---- | --- |
| Hb | $H\beta$ |
| OIII | [OIII] $5006.84$ &angst; |
| Ha | $H\alpha$ |
| NII | [NII] $6583.45$ &angst; |
| SII | [SII] $6719$ + $6731$ &angst; |
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
