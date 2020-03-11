# Compound: N-desalkyl-Itraconazole

## Parameters

Name                                       | Value                  | Value Origin                | Alternative        | Default |
------------------------------------------ | ---------------------- | --------------------------- | ------------------ | ------- |
Solubility at reference pH                 | 1 mg/l                 |                             | No value available | True    |
Reference pH                               | 7                      |                             | No value available | True    |
Lipophilicity                              | 5.1837535822 Log Units |                             | Fit                | True    |
Fraction unbound (plasma, reference value) | 1.1 %                  | Publication-Templeton, 2008 | Templeton, 2008    | True    |
Cl                                         | 2                      |                             |                    |         |
Is small molecule                          | Yes                    |                             |                    |         |
Molecular weight                           | 649.527 g/mol          |                             |                    |         |
Plasma protein binding partner             | Albumin                |                             |                    |         |
## Calculation methods

Name                    | Value               |
----------------------- | ------------------- |
Partition coefficients  | Rodgers and Rowland |
Cellular permeabilities | PK-Sim Standard     |
## Processes

### Metabolizing Enzyme: CYP3A4-Isoherranen 2004

Molecule: CYP3A4
#### Parameters

Name                             | Value                       | Value Origin                 |
-------------------------------- | --------------------------- | ---------------------------- |
In vitro Vmax/recombinant enzyme | 0 nmol/min/pmol rec. enzyme |                              |
Km                               | 0.6284266369 nmol/l         | Publication-Isoherranen 2004 |
kcat                             | 0.0605873508 1/min          | Unknown                      |
### Systemic Process: Glomerular Filtration-GFR

Species: Human
#### Parameters

Name         | Value | Value Origin                 |
------------ | -----:| ---------------------------- |
GFR fraction |     1 | Publication-Isoherranen 2004 |
### Inhibition: CYP3A4-Isoherranen, 2004

Molecule: CYP3A4
#### Parameters

Name | Value       | Value Origin                  |
---- | ----------- | ----------------------------- |
Ki   | 0.32 nmol/l | Publication-Isoherranen, 2004 |
