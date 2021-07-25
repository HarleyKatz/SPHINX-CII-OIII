# SPHINX-CII-OIII

This repository contains the public data release for the [OIII] 88um and [CII] 157um data computed for the sphinx 20 galaxies.

The following data sets are included:
- Relationships between virial mass and [OIII] and [CII] luminosity as a function of redshift and model
- Relationships between SFR and [OIII] and [CII] luminosity as a function of redshift and model

All data sets are in json format with the following structure:
```
{
  redshift: {
    model (solar, core-collapse, core-collapse+): {
      line (CII, OIII): {
        mvir or SFR (virial halo mass, or log10 SFR): List,
        L (log10 L_sun): List
        sig_L: List
      }
    }
  }
}
```
