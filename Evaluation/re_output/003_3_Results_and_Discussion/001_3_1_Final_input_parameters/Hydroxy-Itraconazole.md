# Compound: Hydroxy-Itraconazole

## Parameters

Name                                       | Value           | Value Origin                | Alternative        | Default |
------------------------------------------ | --------------- | --------------------------- | ------------------ | ------- |
Solubility at reference pH                 | 1 mg/l          |                             | No value available | True    |
Reference pH                               | 7               |                             | No value available | True    |
Lipophilicity                              | 3.718 Log Units |                             | Fit                | True    |
Fraction unbound (plasma, reference value) | 1.7 %           | Publication-Templeton, 2008 | Templeton, 2008    | True    |
Cl                                         | 2               |                             |                    |         |
Is small molecule                          | Yes             |                             |                    |         |
Molecular weight                           | 721.633 g/mol   |                             |                    |         |
Plasma protein binding partner             | Albumin         |                             |                    |         |
## Calculation methods

Name                    | Value               |
----------------------- | ------------------- |
Partition coefficients  | Rodgers and Rowland |
Cellular permeabilities | PK-Sim Standard     |
## Processes

### Metabolizing Enzyme: CYP3A4-Isoherranen 2004

Molecule: CYP3A4
Metabolite: Keto-Itraconazole
#### Parameters

Name                             | Value                                  | Value Origin                 |
-------------------------------- | -------------------------------------- | ---------------------------- |
In vitro Vmax/recombinant enzyme | 4.1716224833 nmol/min/pmol rec. enzyme | Publication-Isoherranen 2004 |
Km                               | 4.1716224833 nmol/l                    | Publication-Isoherranen 2004 |
kcat                             | 0.0203370845 1/min                     | Unknown                      |
### Systemic Process: Glomerular Filtration-GFR

Species: Human
#### Parameters

Name         | Value | Value Origin                  |
------------ | -----:| ----------------------------- |
GFR fraction |     1 | Publication-Isoherranen, 2004 |
### Inhibition: CYP3A4-Isoherranen, 2004

Molecule: CYP3A4
#### Parameters

Name | Value       | Value Origin                  |
---- | ----------- | ----------------------------- |
Ki   | 14.4 nmol/l | Publication-Isoherranen, 2004 |
