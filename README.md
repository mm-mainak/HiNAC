# HiNAC: Hidden Neutrino Active Galaxy Candidates
A catalog of selected active galactic nuclei for high-energy neutrino searches.

**Manuscript-linked draft release.** Machine-readable compilation of the **28 AGNs** in Tables 1 and 3 of *Hidden Neutrino Active Galaxy Candidates* (`arXiv:2610.xxxx`). This is an observationally curated candidate catalog, **not** a claim that each object is a detected neutrino emitter.

## Files

- `HiNAC_catalog.csv`: one row per source, combining the two manuscript tables.
- `references.md`: source references and catalog-ID key.
- `selection_criteria.md`: short account of sample construction.

## Data dictionary

- `name`, `swift_id`: names and Swift/BAT designation.
- `sky`: N (declination >= +5°), S (<= −5°), or H (absolute declination < 5°).
- `flux_2_10_1e-12_erg_cm2_s`, `flux_2_195_1e-12_erg_cm2_s`: adopted **intrinsic** energy fluxes, in **10^-12 erg cm^-2 s^-1**.
- `flux_2_10_alternative_1e-12_erg_cm2_s`: independent 2–10 keV estimate printed in parentheses in Table 1; blank where absent. These are *not* measurement uncertainties.
- `rank_2_10`, `rank_2_195`: rankings within this sample for the respective adopted fluxes.
- `gamma_x`: adopted photon index; `log10_nh_cm2`: base-10 log of NH measured in cm^-2.
- `mbh_1e6_msun`: adopted black-hole mass in 10^6 solar masses.
- `mbh_err_minus_1e6_msun`, `mbh_err_plus_1e6_msun`: negative/positive quoted errors in the same units. Blank means **not reported**, not zero.
- `mbh_reference_key`: manuscript Table 1 mass reference letter (see `references.md`).
- `mbh_rescaled_to_adopted_distance`: Y where Table 1 carries the δ mark.
- `distance_mpc`: adopted luminosity distance in Mpc.
- `flux_2_10_inferred_from_14_195`: Y where Table 1 carries an asterisk; these intrinsic 2–10 keV fluxes are inferred from the observed 14–195 keV flux.
- `ra_hms`, `dec_dms`: sexagesimal coordinates from Table 3; `dec_deg`: decimal declination in degrees.
- `lambda_edd`: dimensionless Eddington ratio.
- `seyfert_type`: classification string as printed, including annotations.
- `catalog_id`: provenance ID from Table 3, retained as text.

## Use and citation

Please cite the associated manuscript when using these values. **Bibliographic citation and DOI: to be added once finalized.** Measurement provenance and caveats are documented in the manuscript. No license has yet been selected; choose a suitable data/repository license before public release.

## Versioning

This draft reflects manuscript revision `n/a`.
