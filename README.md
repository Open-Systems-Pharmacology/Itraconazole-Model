# Itraconazole-Model
Whole-body PBPK model of itraconazole. 

**The latest release of this model including a report on model building, model features and model evaluation can be found [here](../../releases/latest).**

<p align="center">
  <img src="Itraconazole.png">
</p> 
This itraconazole model is intended to be used as a perpetrator in CYP3A4-mediated drug-drug interactions. The model includes the sequential metabolites hydroxy-itraconazole, keto-itraconazole and N-desalkyl-itraconazole. All of them are substrates and competitive inhibitors of CYP3A4.

Additional features of the model represent P-gp inhibition.

The model is also suitable for pediatric translations with regard to CYP3A4 ontogeny.

Itraconazole is a triazole agent prescribed for the treatment of fungal infections. It is predominantly metabolized by CYP3A4, resulting in the sequential formation of several metabolites, starting with the major metabolite hydroxy-itraconazole, followed by keto-itraconazole and N-desalkyl-itraconazole. All three metabolites are further metabolized by CYP3A4. Parent and metabolites are reported to competitively inhibit CYP3A4 and hence, are included in the PBPK model. The metabolites inhibit their own formation and itraconazole inhibits further conversion of its metabolites by CYP3A4. Itraconazole has been proposed as one of the most appropriate strong CYP3A4 inhibitors for clinical DDI studies, to replace the no longer recommended CYP3A4 inhibitor drug ketoconazole. 

The presented model is based on the published model by Hanke et al. 2018 [[1](#reference)]. It model was built and evaluated using multiple clinical studies, covering a dose range from 100 to 400 mg after intravenous and oral administration in different formulations, administered under fasted conditions or together with food . Although the plasma concentrations of keto-itraconazole and N-desalkyl-itraconazole are lower than those of itraconazole and hydroxy-itraconazole, N-desalkyl-itraconazole is reported to be a very potent inhibitor in vitro, and integration of the two further metabolites into the model with their inhibitory effects helped to describe the strong nonlinearity and plasma accumulation of itraconazole. The model applies sequential metabolism of itraconazole to hydroxy-itraconazole to keto-itraconazole to N-desalkyl-itraconazole by CYP3A4, including competitive inhibition of CYP3A4 by the parent drug and all three metabolites, and glomerular filtration. Additional features of the model represent P-gp inhibition.

Please note that in comparison to the published version by Hanke et al. 2018 [[1](#References)], the dissolution and solubility has been optimized and updated for the  administration of itraconazole capsules in fasted state.

## Code of conduct

Everyone interacting in the Open Systems Pharmacology community (codebases, issue trackers, chat rooms, mailing lists etc...) is expected to follow the Open Systems Pharmacology [code of conduct](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODE_OF_CONDUCT.md#contributor-covenant-code-of-conduct).

## Contribution

We encourage contribution to the Open Systems Pharmacology community. Before getting started please read the [contribution guidelines](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CONTRIBUTING.md#ways-to-contribute). If you are contributing code, please be familiar with the [coding standard](https://github.com/Open-Systems-Pharmacology/Suite/blob/master/CODING_STANDARDS.md#visual-studio-settings).

## License

The model code is distributed under the [GPLv2 License](https://github.com/Open-Systems-Pharmacology/Suite/blob/develop/LICENSE).

## References
[1] [Hanke N, Frechen S, Moj D, Britz H, Eissing T, Wendl T, Lehr T. PBPK models for CYP3A4 and P-gp DDI prediction: a modeling network of rifampicin, itraconazole, clarithromycin, midazolam, alfentanil and digoxin. CPT Pharmacometrics Syst Pharmacol. 2018 Oct;7(10):647-659.](https://ascpt.onlinelibrary.wiley.com/doi/abs/10.1002/psp4.12343)



