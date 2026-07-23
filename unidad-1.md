setcpm(100) // 140 beat

const PIANO_ON = 1
const PIANO_ON2 = 1
const flute = 1

$piano : note("{<[[b4 g4 e4] [b4 g4 e4] [a4@2 f#4] [d#4 e4 f#4] [b4 g4 e4] [b4 g4 e4] [c5@2 b4] [# a4@2]]@7.5>}") .sound("piano")
.postgain(PIANO_ON ? 0.5 : 0)

$piano : note("{<[[e3]@0.6 [e3, g3, b3]@1.25*2 [b2]@0.6 [eb3, f#3, a3]@1.25*2 [e3]@0.6 [e3, g3, b3]@1.25*2 [a]@0.6 [[eb, a, c] [eb3, f#3, a3]]@1.25]@7.5>}") .sound("piano")
.postgain(PIANO_ON2 ? 0.5 : 0)

$flute : note ("<[e4 g4 b4 a4@1.6 b4@0.5 a4@0.5 g4@0.5 b4@3.2 g4 a4 b4@1.1 e4 g4 b4 a4@1.5 b4@0.5 a4@0.5 g4@0.5 a4 b4 c5@0.95 b4@0.25 c5 b4@2]@15>")
  .sound("gm_acoustic_bass") 
  .postgain(flute ? 1 : 0)
