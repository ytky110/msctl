# Msctl (Music Tools)

## Ideas

- nt: note/tone tool
    - `msctl nt <NOTE> + <half tone>` : 2nd note
    - `msctl nt -w <NOTE> + <whole tone>` : " "
    - `msctl nt <NOTE> - <NOTE>` : number of half tone
    - `msctl nt -w <NOTE> - <NOTE>` : number of whole tone
- in: interval tool
    - `msctl in <NOTE1> <NOTE2>` : interval between NOTE1 and NOTE2
    - `msctl in <NOTE> <Interval Specifier>` : 2nd note
- key: key tool
    - `msctl key <KEY>` : closely related keys
    - `msctl key (<Number of><#/b>)` : key from number of sharps/flats.
- ch: chord tool
    - `msctl ch <KEY> <DEGREE>` : chord of degree DEGREE of key KEY.
    - `msctl ch <KEY> <DEGREE> -4` : same as the previous with 4 notes chords.
    - `msctl ch <NAME> <QUALITY> [INVERSION]` : output notes of the chord.
- cv: convert tool
    - `msctl cv <FROM> <TO>`: convert note names.
        - `en`
        - `nl`
        - `de`
        - `fr`
        - `it`
        - `ja`
        - ...
