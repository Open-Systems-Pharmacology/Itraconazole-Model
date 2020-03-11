# Compound: Keto-Itraconazole

## Parameters

Name                                       | Value                  | Value Origin                | Alternative        | Default |
------------------------------------------ | ---------------------- | --------------------------- | ------------------ | ------- |
Solubility at reference pH                 | 1 mg/l                 |                             | No value available | True    |
Reference pH                               | 7                      |                             | No value available | True    |
Lipophilicity                              | 4.2109086248 Log Units |                             | Fit                | True    |
Fraction unbound (plasma, reference value) | 1 %                    | Publication-Templeton, 2008 | Templeton, 2008    | True    |
Cl                                         | 2                      |                             |                    |         |
Is small molecule                          | Yes                    |                             |                    |         |
Molecular weight                           | 719.617 g/mol          |                             |                    |         |
Plasma protein binding partner             | Albumin                |                             |                    |         |
## Calculation methods

Name                    | Value               |
----------------------- | ------------------- |
Partition coefficients  | Rodgers and Rowland |
Cellular permeabilities | PK-Sim Standard     |
## Processes

### Metabolizing Enzyme: CYP3A4-Isoherranen 2004

Molecule: CYP3A4
Metabolite: N-desalkyl-Itraconazole
#### Parameters

Name                             | Value                            | Value Origin                 |
-------------------------------- | -------------------------------- | ---------------------------- |
In vitro Vmax/recombinant enzyme | 0.0869 pmol/min/pmol rec. enzyme | Publication-Isoherranen 2004 |
Km                               | 2.2214874285 nmol/l              | Publication-Isoherranen 2004 |
kcat                             | 0.3933927416 1/min               | Unknown                      |
### Systemic Process: Glomerular Filtration-GFR

Species: Human
#### Parameters

Name         | Value | Value Origin                 |
------------ | -----:| ---------------------------- |
GFR fraction |     1 | Publication-Isoherranen 2004 |
### Inhibition: CYP3A4-Isoherranen, 2004

Molecule: CYP3A4
#### Parameters

Name | Value       | Value Origin                 |
---- | ----------- | ---------------------------- |
Ki   | 5.12 nmol/l | Publication-Isoherranen 2004 |
