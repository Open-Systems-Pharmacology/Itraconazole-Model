The general concept of building a PBPK model has previously been described by Kuepfer et al. ([Kuepfer 2016](#5-References)) Regarding the relevant anthropometric (height, weight) and physiological parameters (e.g. blood flows, organ volumes, binding protein concentrations, hematocrit, cardiac output) in adults was gathered from the literature and has been previously published ([PK-Sim Ontogeny Database Version 7.3](#5-References)). The information was incorporated into PK-Sim® and was used as default values for the simulations in adults.

The  applied activity and variability of plasma proteins and active processes that are integrated into PK-Sim® are described in the publicly available PK-Sim® Ontogeny Database Version 7.3 ([Schlender 2016](#5-References)) or otherwise referenced for the specific process.

First, a mean model including sequential metabolism of itraconazole to hydroxy-itraconazole to keto-itraconazole to N-desalkyl-itraconazole by CYP3A4 was built using clinical data from single dose and multiple dose studies with intravenous and oral administration (solution, fasted state) of itraconazole. Hereby, competitive inhibition of CYP3A4 was considered for all four compunds. The mean PBPK model was developed using a typical European individual. The relative tissue-specific expressions of enzymes predominantly being involved in the metabolism of midazolam (CYP3A4) were considered. 

The CYP3A4 expression profiles is based on high-sensitive real-time RT-PCR ([Nishimura 2013](#5 References)). Absolute tissue-specific expressions were obtained by considering the respective absolute concentration in the liver. The PK-Sim database provides a default value for CYP3A4 (compare [Rodrigues 1999](#5-References) and assume 40 mg protein per gram liver). 

A specific set of parameters (see below) was optimized using the Parameter Identification module provided in PK-Sim®. Structural model selection was mainly guided by visual inspection of the resulting description of data and biological plausibility.

Once the appropriate structural model was identified, additional parameters for different administration states (*solution fed*, *capsule fasted* and *capsule fed* versus the reference state *solution fasted*) were empirically optimized. Clinical data suggest that the bioavailability of itraconazole is enhanced when an oral solution is given in the fasted state compared to fed state ([Van de Welde 1996](#5-Reference), [Barone 1998a](#5-Reference)). In contradiction, a meal significantly enhances the amount of itraconazole absorbed after administrations of capsules (in comparison to fasted state administrations of capsules) ([Barone 1993a](#5-Reference)). To reflect these observations, parameters like solubility and dissolution kinetics (from capsules) were assumed to be variable between these four scenarios and were independently identified using the Parameter Identification module provided in PK-Sim®.

Details about input data (physicochemical, *in vitro* and clinical) can be found in [Section 2.2](#2.2-Data).

Details about the structural model and its parameters can be found in [Section 2.3](#2.3-Model-Parameters-and-Assumptions).



