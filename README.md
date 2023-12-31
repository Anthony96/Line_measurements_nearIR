Table with the measurements of emission lines observed with JWST/NIRSpec in M-grating mode ($R \simeq 1000$) for CEERS emission line galaxies at redshifts $1 < z < 3$, selected as described in Calabro et al. (2023) : https://arxiv.org/abs/2306.08605 
For any inquiry, contact me at antonello.calabro@inaf.it

# Sample description
The CEERS survey and data are presented in Section 2.1 of Calabro et al. (2023), while the sample selection is described in Section 2.1.3 of the same paper. 
In brief, we select those galaxies in which the spectrum covers at least the $H\beta$ + [OIII] triplet and the $Pa\beta$ + [Fe II] triplet. For the final sample, in addition to the two above triplets, we require the identification of the $H\alpha$ + [N II] triplet and the [S III] $9530$ &angst; line, as the presence of all these lines are essential for the analysis of the optical and near-IR AGN diagnostics presented in the paper. With these criteria, we have selected 65 galaxies between $z= 1$ and $z= 3$, among which 27 galaxies have $z < 1.75$. The table in the repository includes the selected sample, with the addition of $25$ CEERS galaxies (observed in M-grating mode) that do not have **all** the required lines for our work (hence are not selected), but for which we could measure at least the spectroscopic redshift in the same range $1 < z < 3$. The table thus shows measurements for $90$ galaxies in total.

# Table with emission line measurements 

## Methodology
The emission lines are measured with MPFIT (Markwardt et al. 2009) following the procedure explained in Section 2.2 of Calabro et al. (2023). 

The spectroscopic redshift z<sub>spec</sub> and the velocity width $\sigma$ of the lines are determined from the highest S/N emission line (typically $H \alpha$ or [SIII] $9530.62$). **These values are then fixed when fitting the remaining lines**, with a tolerance of $500\ km/s$ and $100\ km/s$, respectively. 

## Results
In this repository we include the table *public_release_line_meas_Calabro23_v1.txt*, with the main properties of the galaxies in the first three columns :

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
| _redshift | - | redshift estimated from the central wavelength of the best-fit gaussian as</br> [ $\lambda$<sub>central</sub>/ $\lambda$<sub>line, restframe</sub> - 1] (only for $H\beta$, $H\alpha$, [SIII] $9530.62$, HeI $10830$, $Pa\beta$, $Pa\alpha$)

**N.B. If the error value is $-1$ (i.e., _flux_err $=-1$), the flux of the corresponding emission line should be treated as an upper limit at $1\sigma$.**
**N.B. For the broad line AGNs selected in the paper, the flux, redshift, and velocity width of permitted lines always refer to the narrow component.**

<hr><hr>
The emission lines fitted and reported in the table are listed below : 


| column prefix | emission line |
| ---- | --- |
| Hb | $H\beta$ |
| OIII_5007 | [OIII] $5006.84$ &angst; |
| Ha | $H\alpha$ |
| NII_6583 | [NII] $6583.45$ &angst; |
| SII | [SII] $6719$ + $6731$ &angst; |
| SIII_9531 | [SIII] $9530.62$ &angst; |
| CI_9850 | [CI]  $9850.26$ &angst; |
| HeI_10830 | HeI $10830$ &angst; |
| PaG | $Pa\gamma$ |
| PII_1188 | [PII] $11882.8$ &angst; |
| FeII_1257 | [FeII] $12566.8$ &angst; |
| PaB | $Pa\beta$ |
| FeII_164 | [FeII] $16435.5$ &angst; |
| PaA | $Pa\alpha$ |
|    |
