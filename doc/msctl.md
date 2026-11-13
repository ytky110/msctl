# Msctl (Music Tools)

An idea.
I don't know in which language I will implement.

## Notation

NOTES:

- `a`
- `ais` / `bes`
- `b`
- `c` / `bes`
- `cis` / `des`
- `d`
- `dis` / `es`
- `e`
- `f` / `eis`
- `fis` / `ges`
- `g`
- `gis` / `as`

KEY:

`<NOTES><Mm>`

CHORD:

`<NOTES><MmAd>[5/6/46]`

## Commands

- nt: note/tone tools
    - `msctl nt + <NOTE> <half tone>` : 2nd note
    - `msctl nt -w + <NOTE> <whole tone>` : " "
    - `msctl nt - <NOTE> <NOTE>` : number of half tone
    - `msctl nt -w - <NOTE> <NOTE>` : number of whole tone
- in: interval tools
    - `msctl in <NOTE1> <NOTE2>` : interval between NOTE1 and NOTE2
    - `msctl in <NOTE> <Interval Specifier>` : 2nd note
- key: key tool
    - `msctl key <KEY>` : Number of #b
    - `msctl key -r <KEY>` : closely related keys
    - `msctl key (<Number of><#/b>)` : key from number of sharps/flats.
- ch: chord tools
    - `msctl ch <CHORD>` OR  
      `msctl ch <-n NAME> <-q QUALITY> [-i INVERSION]` : output notes of the chord.
    - `msctl ch -k <KEY> <DEGREE>` : chord of degree DEGREE of key KEY.
    - `msctl ch -4 <KEY> <DEGREE>` : same as the previous with 4 notes chords.
- cv: convert tools
    - languages:
        - `nl` (default)
        - `en`
        - `de`
        - `fr`
        - `it`
        - `ja`
        - ...
    - `msctl cv [-f FROM] <-t TO> <NOTESTR>` : convert note names.
    - `msctl cv -c <-t TO> <CHORD>` : convert key names.
    - `msctl cv -k <-t TO> <KEY>` : convert key names.
