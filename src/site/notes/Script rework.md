---
{"dg-publish":true,"permalink":"/script-rework/","dgHomeLink":true,"dgPassFrontmatter":false}
---


## Assumptions

1. Every Windows server has to have Cygwin installed
2. All the scheduling is triggered by Crontab / SSH
3. Ideally all the activities (log browsing, script amendment, etc.), are done via 

## Cygwin

1. Install perl package (dependencies perl-base and perl-autobase will be selected automatically)

## Directory

### shl
Contains specific and generic bash scripts

### log
Contains logs, with separated log_acq and log_dsp subdirectories. Each subdirectory has a further spazio subdirectory with the detailed log (/l option of each operation)

### bin
Contains utilities


fdffdfd

![](Drawing%202022-09-07%2022.49.11.excalidraw.svg)
