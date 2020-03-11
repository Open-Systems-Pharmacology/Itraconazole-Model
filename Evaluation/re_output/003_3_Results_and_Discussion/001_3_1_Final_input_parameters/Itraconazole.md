# Compound: Itraconazole

## Parameters

Name                                             | Value                   | Value Origin                                                                                              | Alternative                           | Default |
------------------------------------------------ | ----------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------- | ------- |
Solubility at reference pH                       | 8 mg/l                  | Publication-Taupitz et al. 2013                                                                           | Solution fasted (Taupitz et al. 2013) | True    |
Reference pH                                     | 6.5                     | Publication-Taupitz et al. 2013                                                                           | Solution fasted (Taupitz et al. 2013) | True    |
Solubility at reference pH                       | 1.58 mg/l               |                                                                                                           | Solution fed                          | False   |
Reference pH                                     | 6.5                     |                                                                                                           | Solution fed                          | False   |
Solubility at reference pH                       | 0.9728307177 mg/l       | Parameter Identification-Parameter Identification-Value updated from 'Capsule fasted' on 2019-05-15 12:25 | Capsule fasted                        | False   |
Reference pH                                     | 6.5                     |                                                                                                           | Capsule fasted                        | False   |
Solubility at reference pH                       | 0.7 mg/l                |                                                                                                           | Capsule fed                           | False   |
Reference pH                                     | 6.5                     |                                                                                                           | Capsule fed                           | False   |
Lipophilicity                                    | 4.624 Log Units         | Parameter Identification-Fit                                                                              | Fit                                   | True    |
Fraction unbound (plasma, reference value)       | 0.6016197247 %          |                                                                                                           | Templeton, 2008                       | True    |
Permeability                                     | 0.1111202419 cm/min     | Parameter Identification-Fit                                                                              | Fit                                   | False   |
Specific intestinal permeability (transcellular) | 5.3261558344E-05 dm/min | Parameter Identification-Fit                                                                              | Fit                                   | True    |
Cl                                               | 2                       |                                                                                                           |                                       |         |
Is small molecule                                | Yes                     |                                                                                                           |                                       |         |
Molecular weight                                 | 705.633 g/mol           |                                                                                                           |                                       |         |
Plasma protein binding partner                   | Albumin                 |                                                                                                           |                                       |         |
## Calculation methods

Name                    | Value               |
----------------------- | ------------------- |
Partition coefficients  | Rodgers and Rowland |
Cellular permeabilities | PK-Sim Standard     |
## Processes

### Metabolizing Enzyme: CYP3A4-Isoherranen 2004

Molecule: CYP3A4
Metabolite: Hydroxy-Itraconazole
#### Parameters

Name                             | Value                          | Value Origin                 |
-------------------------------- | ------------------------------ | ---------------------------- |
In vitro Vmax/recombinant enzyme | 0.27 pmol/min/pmol rec. enzyme | Publication-Isoherranen 2004 |
Km                               | 2.0688492598 nmol/l            | Publication-Isoherranen 2004 |
kcat                             | 0.0402937875 1/min             | Unknown                      |
### Systemic Process: Glomerular Filtration-GFR

Species: Human
#### Parameters

Name         | Value | Value Origin                 |
------------ | -----:| ---------------------------- |
GFR fraction |     1 | Publication-Isoherranen 2004 |
### Inhibition: CYP3A4-Isoherranen, 2004

Molecule: CYP3A4
#### Parameters

Name | Value      | Value Origin                               |
---- | ---------- | ------------------------------------------ |
Ki   | 1.3 nmol/l | Parameter Identification-Isoherranen, 2004 |
### Inhibition: ABCB1-Shityakov 2014

Molecule: ABCB1
#### Parameters

Name | Value        | Value Origin               |
---- | ------------ | -------------------------- |
Ki   | 0.008 µmol/l | Publication-Shityakov 2014 |
