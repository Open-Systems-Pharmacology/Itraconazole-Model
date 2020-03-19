### 2.3.1 Absorption

Clinical data suggest that the bioavailability of itraconazole is enhanced when an oral solution is given in the fasted state compared to fed state ([Van de Welde 1996](#5-Reference), [Barone 1998a](#5-Reference)). In contradiction, a meal significantly enhances the amount of itraconazole absorbed after administrations of capsules (in comparison to fasted state administrations of capsules) ([Barone 1993a](#5-Reference)). Thus, four different scenarios can be identified:  *solution fasted*, *solution fed*, *capsule fasted* and *capsule fed*. The *solution fasted* scenario was considered to be the reference scenario.

Herein, the model parameter `Specific intestinal permeability` was optimized to best match clinical data (see  [Section 2.3.5](#2.3.5-Automated-Parameter-Identification)). The default solubility was assumed to be the measured value in the FaSSIF medium (see [Section 2.2.1](#2.2.1-In-vitro-and-physico-chemical-data)).

In a next step, the solubility was optimized for the *solution fed* scenario (in comparison to *solution fasted*).

Then, for the scenarios *capsule fasted* and *capsule fed*, solubility and the dissolution of the capsules (implemented via an empirical Weibull dissolution) were optimized. 

The results of the optimization can be found in [Section 2.3.5](#2.3.5-Automated-Parameter-Identification).

### 2.3.2 Distribution

Various values for the fraction unbound of itraconazole have been reported in literature, ranging from 0.2 to 3.6% (see [Section 2.2.1](#2.2.1-In-vitro-and-physico-chemical-data)). For this model, the final value was optimized within this range to best match observed clinical data (see [Section 2.3.5](#2.3.5-Automated-Parameter-Identification)). For the metabolites, the measured values reported by Riccardi *et al.* ([Riccardi 2015](#5-References)) were incorporated into the model. It was assumed that the major binding partner is albumin.

No pK<sub>a</sub> were reported for the thre metabolites. Here, it was assumed that the metabolites are similar to the parent drug and the reported basic pK<sub>a</sub> value of 3.7 was set (see also [Section 2.2.1](#2.2.1-In-vitro-and-physico-chemical-data))

An important parameter influencing the resulting volume of distribution is lipophilicty. The reported experimental or predicted logP values served asstarting values for the four compounds. Finally, the model parameters `Lipophilicity` were optimized to match best clinical data (see also [Section 2.3.5](#2.3.5-Automated-Parameter-Identification)).

After testing the available organ-plasma partition coefficient and cell permeability calculation methods built in PK-Sim, observed clinical data was best described by choosing the partition coefficient calculation by `Rodgers and Rowland` and cellular permeability calculation by `PK-Sim Standard ` for itraconazole and its metabolites.

### 2.3.3 Metabolism and Elimination

Two sequential metabolic pathway via CYP3A4 were implement into the model via Michaelis-Menten kinetics for all four compounds. *In vitro* determined unbound K<sub>m</sub> values ([Isoherranen 2004](#5-References)) served as starting values (if available) . Respective k<sub>cat</sub> values were optimized to best match clinical data (see also [Section 2.3.5](#2.3.5-Automated-Parameter-Identification)).

The CYP3A4 expression profiles is based on high-sensitive real-time RT-PCR ([Nishimura 2013](#5 References)). Absolute tissue-specific expressions were obtained by considering the respective absolute concentration in the liver. The PK-Sim database provides a default value for CYP3A4 (compare [Rodrigues 1999](#5-References) and assume 40 mg protein per gram liver). 

Additionally, for all four compounds a renal clearance (assumed to be driven by glomerular filtration) was implemented.

### 2.3.4 DDI Parameters

The following sub-sections describe the model's input for DDI-related parameters, i.e. inhibition on certain enzymes and transporters, for which itraconazole may act in a perpetrator role. Verification of these model parameters and linked processes in combination with sensitive CYP3A4 / P-gp substrates is not evaluated in this report. Applications are assessed in specific use cases and reported elsewhere. Note, however, that the competitive CYP3A4 inhibition of the four compounds results in inhibition of metabolite formation (of hydroxy-itraconazole, keto-itraconazole, N-desalkyl-itraconazole) and the metabolism of N-desalkyl-itraconazole. This effectively contributes to the PK non-linearity of itraconazole and its metabolites, especially after multiple doses.

#### CYP3A4 inhibition
*In vitro* determined unbound K<sub>i</sub> values for itraconazole and hydroxy-itraconazole ([Isoherranen 2004](#5-References)) served directly as model input (see [Section 2.2.1](#2.2.1-In-vitro-and-physico-chemical-data)).

*In vitro* determined unbound IC<sub>50</sub> values for keto-itraconazole and N-desalkyl-itraconazol ([Isoherranen 2004](#5-References)) were converted to K<sub>i</sub>  values via Cheng-Prusoff equation ([Chen 1973](#5-References)) with a substrate (*midazolam*) concentration of 1 µmol/L and an assumed substrate (*midazolam*) K<sub>m</sub> value of 2.73 µmol/L (see [Section 2.2.1](#2.2.1-In-vitro-and-physico-chemical-data)).

#### P-gp inhibition
An *in vitro* determined K<sub>i</sub> values for itraconazole ([Shityakov 2014](#5-References)) served directly as model input (see [Section 2.2.1](#2.2.1-In-vitro-and-physico-chemical-data)).



### 2.3.5 Automated Parameter Identification

This is the result of the final parameter identification for the basic model:

| Compound        | Model Parameter                              | Optimized Value                                              | Unit      |
| --------------- | -------------------------------------------- | ------------------------------------------------------------ | --------- |
| Itraconazole    | `Lipophilicity`                              | 4.62                                                         | Log Units |
|                 | `Specific intestinal permeability`           | 5.33E-05                                                     | dm/min    |
|                 | `Fraction unbound (plasma, reference value)` | 0.6                                                          | %         |
|                 | `Km` (CYP3A4)                                | 2.07                                                         | nmol/L    |
|                 | `kcat` (CYP3A4)                              | 0.040                                                        | 1/min     |
| Hydroxy-Itr.    | `Lipophilicity`                              | 3.72                                                         | Log Units |
|                 | `Fraction unbound (plasma, reference value)` | 1.7 FIXED (see [Section 2.2.1](#2.2.1-In-vitro-and-physico-chemical-data)) | %         |
|                 | `Km` (CYP3A4)                                | 4.17                                                         | nmol/L    |
|                 | `kcat` (CYP3A4)                              | 0.020                                                        | 1/min     |
| Keto-Itr.       | `Lipophilicity`                              | 4.21                                                         | Log Units |
|                 | `Fraction unbound (plasma, reference value)` | 1.0 FIXED (see [Section 2.2.1](#2.2.1-In-vitro-and-physico-chemical-data)) | %         |
|                 | `Km` (CYP3A4)                                | 2.22                                                         | nmol/L    |
|                 | `kcat` (CYP3A4)                              | 0.393                                                        | 1/min     |
| N-Desalkyl-Itr. | `Lipophilicity`                              | 5.18                                                         | Log Units |
|                 | `Fraction unbound (plasma, reference value)` | 1.1 FIXED (see [Section 2.2.1](#2.2.1-In-vitro-and-physico-chemical-data)) | %         |
|                 | `Km` (CYP3A4)                                | 0.63                                                         | nmol/L    |
|                 | `kcat` (CYP3A4)                              | 0.061                                                        | 1/min     |



This is the result of the final parameter identification for the solubility (and dissolution parameters of an empirical Weibull function) in case of capsule administrations) for the different administration scenarios of itraconazole:

| Scenario        | Model Parameter                    | Optimized Value                                              | Unit |
| --------------- | ---------------------------------- | ------------------------------------------------------------ | ---- |
| Solution fasted | `Solubility at reference pH`       | 8.0 FIXED (see [Section 2.2.1](#2.2.1-In-vitro-and-physico-chemical-data)) | mg/L |
| Solution fed    | `Solubility at reference pH`       | 1.58                                                         | mg/L |
| Capsule fasted  | `Solubility at reference pH`       | 0.97                                                         | mg/L |
|                 | `Dissolution time (50% dissolved)` | 406                                                          | min  |
|                 | `Dissolution shape`                | 1.43                                                         |      |
| Capsule fed     | `Solubility at reference pH`       | 0.70                                                         | mg/L |
|                 | `Dissolution time (50% dissolved)` | 139                                                          | min  |
|                 | `Dissolution shape`                | 0.82                                                         |      |