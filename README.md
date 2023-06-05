# CGMech

Zipfile containing the 1700 txts: on [Google Drive](https://drive.google.com/file/d/1WUarJpC83vojDsEYpECCgjLxn6ubJYj6/view?usp=share_link)

| Commit | Accuracy | Excel | Comments |
| --- | --- | --- | --- |
| 0 | 76.18% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lDUfyg3LlImTEhXd?e=c2TJZj) | Cat[high/low/middle] - Tokenizer needs fixing: numbers and punct. |
| 1 | 75.00% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lDnJfBP-e2P7FCoF?e=pmr5uZ) | Cat [high/low/middle] - LogReg, Tokenizer fixed |
| 2 | 55.00% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lDuxE4w5Led5wV1o?e=ublfZC) | Proxy [1-10] - LogReg|
| 3 | 75.00% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lD_4DfAEYRd1QoIP?e=q0NrAA) | Cat [high/low/middle] - LinearSVC classifier|
| 4 | 61.18% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lD3vYhnTTCah6R2b?e=8UWcxU) | Proxy [1-10] - LinearSVC classifier|
| 5 | 31.18% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lEFWpl4-Aw-1sV2I?e=KwrnCA) | Proxy [1-10] - LinearSVC, RemoveFrequentTokens 0.10 too high, =baserate|
| 6 | 31.00% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lEOgbtfuNZuFSe6u?e=subzvx) | Proxy [1-10], RemoveFrequentTokens 0.05 too high, with ImportantWords [w*:0.5]
| 7 | 31.180% | No Link | Proxy [1-10], RemoveFrequentTokens needs fixing (0.2)
| 8 | 62.65% | No Link | Proxy [1-10], no RemoveFrequent, with ImportantWords (w:0.5), Extracted token with coef needs fixing
| 9 | 61.18% | No Link | Proxy [1-10], remove 0.5% most frequent (fixed), with important words (w:0.5), no tokens with coef
| 10 | 61.18% | No Link | Proxy [1-10], remove 0.5% most frequent (fixed), with important words (w:0.1), no tokens with coef
| 11 | 61.18% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lG2sM_05W7u2-mvg?e=x4WZl7) | no RemoveFrequent, with important words (w:0.1)
| 12 | 61.18% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lF0P9xDX5Ewje1xx?e=MhCnsm) | no RemoveFrequent, with important words w:0.5 -> same results!
| 13 | --- | No Link | 1st try gridsearch for optimizing ImportantWords weight --> takes too much ressource
| 14 | --- | No Link | 2nd try gridsearch, train on 20% dataset --> still too much ressource
| 15 | 61.59% | [Link](https://1drv.ms/x/s!AuVPkhSveTP3lgSfvGeFzapXRIV5?e=6HsOjQ) | NEW DATASET - "auto" train, no important words, 2h37




