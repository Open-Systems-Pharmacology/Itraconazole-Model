### 2.2.1 In vitro and physico-chemical data

A literature search was performed to collect available information on physical chemical properties of itraconazole and metabolites. The obtained information from literature is summarized in the table below, and is used for model building.

#### Itraconazole

| **Parameter**                         | **Unit**                   | **Value**      | Source                            | **Description**                                 |
| :------------------------------------ | -------------------------- | -------------- | --------------------------------- | ----------------------------------------------- |
| MW                                    | g/mol                      | 705.633        | [DrugBank DB01167](#5-References) | Molecular weight                                |
| pK<sub>a,base</sub>                   |                            | 3.7            | [Heykants 1989](#5-References)    | Basic dissociation constant                     |
| Solubility (pH)                       | mg/L                       | 8.0<br />(6.5) | [Taupitz 2013](#5 References)     | FaSSIF solubility                               |
| logP                                  |                            | 5.66           | [Heykants 1989](#5-References)    | Partition coefficient between octanol and water |
| fu                                    | %                          | 0.2            | [Heykants 1989](#5-References)    | Fraction unbound in plasma                      |
|                                       | %                          | 0.2            | [Riccardi 2015](#5-References)    | Fraction unbound in plasma                      |
|                                       | %                          | 1.58           | [Ishigam 2001](#5-References)     | Fraction unbound in plasma                      |
|                                       | %                          | 3.6            | [Templeton 2008](#5-References)   | Fraction unbound in plasma                      |
| V<sub>max</sub>, K<sub>m</sub> CYP3A4 | pmol/min/nmol,<br />nmol/L | 270<br />3.9   | [Isoherranen 2004](#5-References) | CYP3A4 supersomes Michaelis-Menten kinetics     |
| K<sub>i</sub> CYP3A4                  | nmol/L                     | 1.3            | [Isoherranen 2004](#5-References) | CYP3A4 inhibition constant                      |
| K<sub>i</sub> P-gp                    | nmol/L                     | 8.0            | [Shityakov 2014](#5-References)   | P-gp inhibition constant                        |



#### Hydroxy-Itraconazole

| **Parameter**                         | **Unit**                   | **Value**   | Source                               | **Description**                                              |
| :------------------------------------ | -------------------------- | ----------- | ------------------------------------ | ------------------------------------------------------------ |
| MW                                    | g/mol                      | 721.633     | [DrugBank DBMET00374](#5-References) | Molecular weight                                             |
| logP                                  |                            | 4.5         | [PubChem CID 108222](#5-References)  | Partition coefficient between octanol and water, computed by XLogP3 3.0 |
| fu                                    | %                          | 0.5         | [Templeton 2008](#5-References)      | Fraction unbound in plasma                                   |
|                                       | %                          | 1.7         | [Riccardi 2015](#5-References)       | Fraction unbound in plasma                                   |
|                                       | %                          | 2.12        | [Chen 2016](#5-References)           | Fraction unbound in plasma                                   |
| V<sub>max</sub>, K<sub>m</sub> CYP3A4 | pmol/min/nmol,<br />nmol/L | 543<br />27 | [Isoherranen 2004](#5-References)    | CYP3A4 supersomes Michaelis-Menten kinetics                  |
| K<sub>i</sub> CYP3A4                  | nmol/L                     | 14.4        | [Isoherranen 2004](#5-References)    | CYP3A4 inhibition constant                                   |



#### Keto-Itraconazole

| **Parameter**                         | **Unit**                   | **Value**     | Source                                | **Description**                                              |
| :------------------------------------ | -------------------------- | ------------- | ------------------------------------- | ------------------------------------------------------------ |
| MW                                    | g/mol                      | 719.617       | [PubChem CID 53865186](#5-References) | Molecular weight                                             |
| logP                                  |                            | 4.5           | [PubChem CID 53865186](#5-References) | Partition coefficient between octanol and water, computed by XLogP3 3.0 |
| fu                                    | %                          | 1.0           | [Riccardi 2015](#5-References)        | Fraction unbound in plasma                                   |
|                                       | %                          | 5.3           | [Templeton 2008](#5-References)       | Fraction unbound in plasma                                   |
| V<sub>max</sub>, K<sub>m</sub> CYP3A4 | pmol/min/nmol,<br />nmol/L | 86.9<br />1.4 | [Isoherranen 2004](#5-References)     | CYP3A4 supersomes Michaelis-Menten kinetics                  |
| IC<sub>50</sub> CYP3A4<sup>†</sup>    | nmol/L                     | 7.0           | [Isoherranen 2004](#5-References)     | CYP3A4 inhibition constant for half maximal inhibitory concentration at constant substrate concentration |

<sup>†</sup> The IC<sub>50</sub> values was converted to a K<sub>i</sub> value via Cheng-Prusoff equation ([Chen 1973](#5-References)) with a substrate (*midazolam*) concentration of 1 µmol/L and an assumed substrate (*midazolam*) K<sub>m</sub> value of 2.73 µmol/L: **5.12 nmol/L**



#### N-Desalkyl-Itraconazole

| **Parameter**                      | **Unit** | **Value** | Source                                | **Description**                                              |
| :--------------------------------- | -------- | --------- | ------------------------------------- | ------------------------------------------------------------ |
| MW                                 | g/mol    | 649.527   | [PubChem CID 53789808](#5-References) | Molecular weight                                             |
| logP                               |          | 4.2       | [PubChem CID 53789808](#5-References) | Partition coefficient between octanol and water, computed by XLogP3 3.0 |
| fu                                 | %        | 1.1       | [Riccardi 2015](#5-References)        | Fraction unbound in plasma                                   |
|                                    | %        | 1.2       | [Templeton 2008](#5-References)       | Fraction unbound in plasma                                   |
| IC<sub>50</sub> CYP3A4<sup>†</sup> | nmol/L   | 0.44      | [Isoherranen 2004](#5-References)     | CYP3A4 inhibition constant for half maximal inhibitory concentration at constant substrate concentration |

<sup>†</sup> The IC<sub>50</sub> values was converted to a K<sub>i</sub> value via Cheng-Prusoff equation ([Chen 1973](#5-References)) with a substrate (*midazolam*) concentration of 1 µmol/L and an assumed substrate (*midazolam*) K<sub>m</sub> value of 2.73 µmol/L: **0.32 nmol/L**



### 2.2.2 Clinical data

A literature search was performed to collect available clinical data on itraconazole and its metabolite in adults. The itraconazole model was built and verifified using various clinical studies, covering a dosing range from 100 to 200 mg in different formulations (solution *vs.* capsule), administered under fasted conditions or together with food.

The following dosing senarios were simulated and compared to respective data:

| Route | Formulation | Food state | Dose<br />[mg] | Dosing | PK Data                                                      | Used for<sup>†</sup> | Reference                          |
| ----- | ----------- | ---------- | -------------- | ------ | ------------------------------------------------------------ | -------------------- | ---------------------------------- |
| iv    | -           | -          | 100            | SD     | Itraconazole                                                 | mv                   | [Heykants  1989](5-References)     |
|       |             |            | 200            | OD     | Itraconazole<br />Hydroxy-Itr.                               | mbb                  | [Mouton  2006](5-References)       |
| po    | solution    | fasted     | 100            | SD     | Itraconazole                                                 | mbb                  | [Van de  Velde 1996](5-References) |
|       |             |            |                |        | Itraconazole<br />Hydroxy-Itr.                               | mbb                  | [Van  Peer 1989](5-References)     |
|       |             |            |                | OD     | Itraconazole<br />Hydroxy-Itr.<br />Keto-Itr.<br />N-Desalkyl-Itr. | mbb                  | [Templeton  2008](5-References)    |
|       |             |            | 200            | OD     | Itraconazole<br />Hydroxy-Itr.                               | mbb                  | [Barone  1998a](5-References)      |
|       |             | fed        | 100            | SD     | Itraconazole<br />Hydroxy-Itr.                               | mbe                  | [Van de  Velde 1996](5-References) |
|       |             |            |                |        | Itraconazole                                                 | mbe                  | [Heykants  1989](5-References)     |
|       |             |            | 200            | SD     | Itraconazole<br />Hydroxy-Itr.                               | mbe                  | [Barone  1998b](5-References)      |
|       |             |            |                | OD     | Itraconazole<br />Hydroxy-Itr.                               | mbe                  | [Barone  1998a](5-References)      |
|       | capsule     | fasted     | 100            | SD     | Itraconazole                                                 | mbe                  | [Van  Peer 1989](5-References)     |
|       |             |            |                | BID    | Itraconazole                                                 | mv                   | [Kivistö 1997](5-References)       |
|       |             |            | 200            | SD     | Itraconazole<br />Hydroxy-Itr.                               | mbe                  | [Barone  1993](5-References)       |
|       |             |            |                | OD     | Itraconazole                                                 | mbe                  | [Jalava  1997](5-References)       |
|       |             |            |                | OD     | Itraconazole                                                 | mbe                  | [Olkkola  1994](5-References)      |
|       |             | fed        | 100            | SD     | Itraconazole                                                 | mbe                  | [Van Peer  1989](5-References)     |
|       |             |            |                | OD     | Itraconazole                                                 | mbe                  | [Van Peer  1989](5-References)     |
|       |             |            |                |        | Itraconazole                                                 | mv                   | [Hardin  1988](5-References)       |
|       |             |            | 200            | SD     | Itraconazole<br />Hydroxy-Itr.                               | mbe                  | [Barone  1993](5-References)       |
|       |             |            |                |        | Itraconazole<br />Hydroxy-Itr.                               | mbe                  | [Barone  1998b](5-References)      |
|       |             |            | 200            | OD     | Itraconazole                                                 | mv                   | [Hardin  1988](5-References)       |
|       |             |            |                | BID    | Itraconazole                                                 | mbe                  | [Barone  1993](5-References)       |
|       |             |            |                |        | Itraconazole<br />Hydroxy-Itr.                               | mv                   | [Hardin  1988](5-References)       |

<sup>†</sup> *mbb* model building basic: used to inform the basic model parameters (see [Section 2.3.4](#2.3.4-Automated-Parameter-Identification)); *mbe* model building extended: used to inform solubility (and formulation-depenendent) parameter only (see [Section 2.3.4](#2.3.4-Automated-Parameter-Identification)); *mv* model verification only



