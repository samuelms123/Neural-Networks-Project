# IRMAS Dataset

Reference:  
Bosch, J. J., Janer, J., Fuhrmann, F., & Herrera, P. “A Comparison of Sound Segregation Techniques for Predominant Instrument Recognition in Musical Audio Signals”, in Proc. ISMIR (pp. 559-564), 2012  

Website: [https://www.upf.edu/web/mtg/irmas](https://www.upf.edu/web/mtg/irmas)

---

## Instruments

```python
'cel': 'Celesta',
'cla': 'Clarinet',
'flu': 'Flute',
'gac': 'Acoustic Guitar',
'gel': 'Electric Guitar',
'org': 'Organ',
'pia': 'Piano',
'sax': 'Saxophone',
'tru': 'Trumpet',
'vio': 'Violin',
'voi': 'Human Voice'
```

## Training set

Each train excerpt has one target instrument.

Naming conventions vary a bit, but first brackets always tell the target instrument in the clip.

Examples from the set:

'228__[pia][nod][pop_roc]1437__1.wav'
    PIANO, NODRUMS, POP ROCK

'207__[voi][dru][cou_fol]2414__3.wav'
    HUMAN VOICE, DRUMS, COUNTRY FOLK

'[cel][cla]0080__1.wav'
    CELESTA, CLASSICAL

Amount of audio files per instrument:

{'cel': 388, 'cla': 505, 'flu': 451, 'gac': 637, 'gel': 760, 'org': 682, 'pia': 721, 'sax': 626, 'tru': 577, 'vio': 580, 'voi': 778}

Each audio file is excerpt of 3 seconds from over 2000 distinct recordings.

## Testing sets

Total of 3 testing folders containing 2874 audio files.

Test audio files are 5-20 second excerpts from complete songs. Total audio length combined is ~13 hours.

Each audio file has 1-5 instruments present.

Each audio file is followed by a .txt file that includes the instruments present in the file.

For example:

'01 - Inolvidable-3.txt'
'01 - Inolvidable-3.wav'

cat '01 - Inolvidable-3.txt'
pia
voi

Amount of audio clips that have n instruments: {n, clips_amount}:

Testing part1: {1: 302, 2: 396, 3: 98, 4: 11}
Testing part2: {1: 578, 2: 567, 3: 132, 4: 22, 5: 2}
Testing part3: {1: 356, 2: 315, 3: 88, 4: 6, 5: 1}