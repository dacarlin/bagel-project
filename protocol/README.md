# Laboratory protocols for production and assay of β-glucosidase B

The characterization of point mutants of β-glucosidase B from *P. polymxa* ("Bagel") is an ongoing project in the Siegel group. This repository contains all the laboratory protocols for the production and assay.

+ We use an automated Kunkel mutagenesis procedure that runs on [Transcriptic's workcell](https://www.transcriptic.com/). Single-stranded DNA for this protocol is available for free from our lab, please email us. If you would like to perform this procedure by hand, you can follow [the Siegel group protocol for a manual Kunkel mutagenesis procedure](https://docs.google.com/a/ucdavis.edu/folderview?usp=sharing&id=0B3zIXvOOrmpqcEM5WWRadThsVUE).

The following protocols are used in our lab:

+ `production_production` for production of protein beginning from purified plasmid
+ `gel_and_yields` for determining protein purity by SDS-PAGE and protein yield by A280
+ `kinetic_assay` for determining Michaelis-Menten parameters from a plate assay (also see [data analysis tools](bagel-fitter))
+ `thermal_stability_assay` for an assay to determine an enzyme's melting temperature

The entire pipeline:

+ deep prep from `stock_recipes.md`
+ `ssDNA_prep.md` for preparation of single-stranded DNA template
+ [automated Kunkel mutagenesis on Transcriptic](TSKunkel)
+ `protein_production.md`
+ `gel_and_yields.md` (and, if necessary, production again)
+ `kinetic_assay.md`
+ `thermal_stability_assay.md`
+ [data analysis](bagel.genomecenter.ucdavis.edu) using [a custom web app](bagel-fitter) and provided Jupyter Notebooks

The outputs for each protein are the soluble expression (yes/no), quantitative protein yield by A280 (in units of mg/mL), the Michaelis-Menten constants *k*<sub>cat</sub> and K<sub>M</sub>, and the melting temperature (T<sub>m</sub>).

Data for the native BglB sequence:

Mutant|Protein yield (mg/mL)|Expression (1=yes, 0=no)|*k*<sub>cat</sub> (1/min)|Percent error, *k*<sub>cat</sub>|K<sub>M</sub> (mM)|Percent error, K<sub>M</sub>|T<sub>m</sub> (C)
---|---|-----|-----|-----|-----|-----|-----
BglB|1.13|1|895.6|2.1|4.79|9.8|39.6
