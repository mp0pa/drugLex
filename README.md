# drugLex
drugLex is the first comprehensive multi-dimensional dataset of drug-related terminology to also include prescription drugs with a potential of abuse. Accounting for both pharmaceutical and street names of 48 distinct drug categories, it aims to bridge the gap between clinical use cases and mentions of substance use in online communities. Manually curated and reviewed, it is designed for NLP and/or data science tasks.

## Datasets
| File | Description |
| :--- | :--- |
| `DruglexFull.csv` | The reference dataset. Includes names of chemicals, brand/generic prescription drug names, and all identified street aliases (e.g., *Addie, benzos, Ozempic*). Research chemicals, or designer drugs without known street names were omitted. Also contains a list of terms with a high likelihood of co-occurrence.|
| `DruglexMini.csv` | A curated subset containing only **context-independent, non-ambiguous** street names to reduce false positives in NLP tasks. |
| `ExplicitVSClean.csv` | Pairwise sentence list for lexical translation/censoring. "Clean" versions are primarily derived via rhyming slang and euphemisms. |
| `DrugsInContext.csv` | A corpus of **27,544 lines** of Reddit/Twitter comments and forum threads where drug use is discussed in informal settings. |

---
## Methodology

### Data Sourcing & Validation
The lexicon was compiled through a rigorous cross-referencing process of both law-enforcement agencies acts and threads originating from substance use online communities:
* **Official Reports:** DEA 2018 Drug Slang Intelligence Report, Dutch Opioid State Act (for "Hard Drug" classification), and the DEA Resource Guide.
* **Online Communities:** Targeted parsing of subreddits (e.g., `r/opiates, r/Drugs`) and contextual sampling from the **Erowid LSA Dataset** (see [GitHub Repository](https://github.com/Monkeyanator/erowid-lsa/tree/master)).
* **Linguistic Resources:** Wiktionary and specialized health glossaries (Black Bear Rehab, NSW Health, Addiction Center, ChildHealthBC).
* **Pop Culture trends:** Manual inclusion of modern/emerging terms such as **Ozempic** and prescription nicknames like **Vikes**.

---
## License, Ethics, Acknowledgements

### Licence: This dataset is released under the **Creative Commons Zero v1.0 Universal (CC0)**. You may copy, modify, and distribute the work, even for commercial purposes, without asking permission.

### Ethical Statement
This dataset is provided for **Linguistic Research, Natural Language Processing (NLP), and Harm Reduction** purposes only. It does not promote or encourage the use of illicit substances in any way, shape or form.

## Acknowledgements: If you use this dataset, please cite the present DrugLex repository.

