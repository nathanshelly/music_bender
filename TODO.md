# TODO

## First Stage - MVP

- [x] Get modulation of volume, pitch & filter
- [x] Create control scheme of start gestures (for now just swipe left/right/up/down) & end gesture (clenched fist) and see them reliably trigger
  - [x] bang on extracted circle/swipe
  - [x] bang on clenched fist
- [x] On start gesture begin modulation of corresponding parameter
  - if swipe detected then turn on that modulation (essentially just route signal through or around that feature, currently no stacking so just a simple switch)
  - if clenched fist send signal uninterrupted

## Second Stage - Multiple Modulators

### TONIGHT

- [x] Stackable modulation
- [x] Use number of fingers on right hand + clenched left fist to begin - gives six modulatable parameters
  - [x] pitch
  - [x] volume
  - [x] filter

### TOMRORROW

- [ ] Save last value on normal parameter exit
- [ ] Add exit mode gesture - both fists clenched
- [ ] few more parameters
  - [ ] reverb
  - [ ] chorus/echoes

## Future

- [ ] - Allow movement in time (scrub back and forth, building up looped effects)
- [ ] - Allow specifying dimension of control for parameter
