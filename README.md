# CGMech

Zipfile containing the 1700 txts: on [Google Drive](https://drive.google.com/file/d/1WUarJpC83vojDsEYpECCgjLxn6ubJYj6/view?usp=share_link)

| Commit | Accuracy | Excel | Comments |
| --- | --- | --- | --- |
| 0 | 76.18% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lDUfyg3LlImTEhXd?e=c2TJZj) | Cat[high/low/middle] - Tokenizer needs fixing: numbers and punct. |
| 1 | 75.00% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lDnJfBP-e2P7FCoF?e=pmr5uZ) | Cat [high/low/middle] - LogReg, Tokenizer fixed |
| 2 | 55.00% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lDuxE4w5Led5wV1o?e=ublfZC) | Proxy [1-10] - LogReg|
| 3 | 75.00% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lD_4DfAEYRd1QoIP?e=q0NrAA) | Cat [high/low/middle] - LinearSVC classifier|
| 4! | 61.18% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lD3vYhnTTCah6R2b?e=8UWcxU) | Proxy [1-10] - LinearSVC classifier|
| 5 | 31.18% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lEFWpl4-Aw-1sV2I?e=KwrnCA) | Proxy [1-10] - LinearSVC, RemoveFrequentTokens 0.10 too high, =baserate|
| 6 | 31.00% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lEOgbtfuNZuFSe6u?e=subzvx) | Proxy [1-10], RemoveFrequentTokens 0.05 too high, with ImportantWords [w*:0.5]
| 7 | 31.180% | No Link | Proxy [1-10], RemoveFrequentTokens needs fixing (0.2)
| 8 | 62.65% | No Link | Proxy [1-10], no RemoveFrequent, with ImportantWords (w:0.5), Extracted token with coef needs fixing
| 9 | 61.18% | No Link | Proxy [1-10], remove 0.5% most frequent (fixed), with important words (w:0.5), no tokens with coef
| 10 | 61.18% | No Link | Proxy [1-10], remove 0.5% most frequent (fixed), with important words (w:0.1), no tokens with coef
| 11 | 61.18% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lG2sM_05W7u2-mvg?e=x4WZl7) | no RemoveFrequent, with important words (w:0.1)
| 12 | 61.18% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lF0P9xDX5Ewje1xx?e=MhCnsm) | no RemoveFrequent, with important words w:0.5 -> same results!
| 13 | --- | No Link | 1st try gridsearch for optimizing ImportantWords weight -> takes too much ressource
| 14 | --- | No Link | 2nd try gridsearch, train on 20% dataset -> still too much ressource
| 15 | 61.59% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lgSfvGeFzapXRIV5?e=6HsOjQ) | NEW DATASET - "auto" train, no important words
| 16 | 61.59% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lgaTl7h_DEwoY2En?e=cSyghj) | With ImportantWords (w:custom) -> no improvement!
| 17 | --- | [Link](https://github.com/stephanevez/CGMech/blob/7fa7dd80b5cbd79ed0d2154d94a6e6a6bd0f2bf6/SpacyEntities.txt) | Entity detection with spacy: failed
| 18! | 65.08% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3liNksMVtPJpuSWqK?e=JL2Ldk) | include 2-grams -> accuracy improves
| 19 | 61.27% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lir2vwrGynSrZt4h?e=o1hsQX) | 1-word tokens, ignore_companies -> worse
| 20 | 61.27% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3ljMaG5cDEXgvmvFn?e=qoMYkk) | 1-word tokens, ignore_companiesv2 -> still no improvement
| 21 | 61.59% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3ljHzaIlVwRcinksL?e=bzqFij) | 1-word tokens, ignore_foreign -> baseline
| 22! | 62.86% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3li9StthyhuSdlc58?e=0pTW25) | 1-word tokens, ignore_abbrev -> accuracy improves
| 23 | 61.59% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3ljVUciHyYsjgZdip?e=YleMv4) | 1-word tokens, ignore_locations -> baseline
| 24 | 61.59% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3ljf0zwN2qmwxDG82?e=vfpnWv) | 1-word tokens, ignore_surnames -> baseline
| 25 | 62.86% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3ljn_OlI1dRLgV-dH?e=udacEs) | 1-word tokens, ignore_foreign+ignore_abbrev -> same as 22
| 26 | pending | [Link]() | 1-word tokens, ignore_foreign+ignore_abbrev+ignore_companiesv2
| 27 | 62.86% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3ljtwb3wnty3aCcw2?e=iNQKJK) | 1-word tokens, ignore_foreign+ignore_abbrev+ignore_locations -> same as 22
| 28 | 62.86% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3ljxndS1UxtQ72d9c?e=TpnSWc) | 1-word tokens, ignore_foreign+ignore_abbrev+ignore_surnames -> same as 22
| 29 | 25.40% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lkMkVBGyQNTuu1XR?e=NQyZTK) | 2-grams, ignore_foreign+ignore_abbrev+ignore_surnames+ignore_locations+ignore_companiesv2 -> need fixing
| 30 | 46.35% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lkQ38TEDdQEVshwq?e=xJbIUI) | 2-grams, ignore_foreign+ignore_abbrev+ignore_surnames+ignore_locations+ignore_companiesv2 -> need fixing







