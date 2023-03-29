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
| 7 | PENDING.00% | [Link]() | Proxy [1-10], RemoveFrequentTokens 0.02
| 8 | PENDING.00% | [Link]() | Proxy [1-10], no RemoveFrequent, with ImportantWords (w:0.5)
