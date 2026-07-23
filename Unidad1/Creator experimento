setcpm(100)

const PIANO_ON = 1
const PIANO_ON2 = 1
const COSO = 1

$piano : note(`<[[[e6 g6 b6]@16 a6@8 [b6 a6 g6]@9 b6@12.5 ~ ~ ~] [~ [e6 f#6 g6]@20 a6@10 ~ ~ g6@4 ~ ~ f#6@3.5 ~ ~ ~ g6@4 ~ ~ ~ ~ f#6@6]]@20
               [[~]]@2
               
               [[[b6 g6 e6] [b6 g6 e6] [a6@2 f#6] [d#6 e6 f#6] [b6 g6 e6] [b6 g6 e6] [c7@2 b6] [~ a6@2]]*3]@22.5 [[~]]@30>`) 
  .sound("piano")
  .coarse(4) 
  .postgain(PIANO_ON ? 0.75 : 0)  
  

$piano : note(`<[e5@3 b4 eb5 f#5 e5 g5 b5 g5 e5 c5 a4 c5 e5 b4 eb5 f#5]@20 [[~]]@9.5 

                [[[e3, e2]@0.6 [e3, g3, b3]@1.25*2 [b2]@0.6 [eb3, f#3, a3]@1.25*2 
                [e3]@0.6 [e3, g3, b3]@1.25*2 [a]@0.6 [[eb, a, c] [eb3, f#3, a3]]@1.25]*6]@45>`) 
  .sound("piano")  
  .postgain(PIANO_ON2 ? 0.5 : 0) 
  

$coso : note(`<[[~]]@44.5 [[e4 g4 b4 a4@1.6 b4@0.5 a4@0.5 g4@0.5 b4@3.2 g4 a4 b4@1.1 e4 g4 b4 a4@1.5 b4@0.5 a4@0.5 g4@0.5 a4 b4 c5@0.95 b4@0.25 c5 b4@2]*2]@30>`)
  .sound("gm_acoustic_bass")
  .lpf(3500)
  .hpf(120)
  .room(0.35)
  .delay(0.15)
  .postgain(COSO ? 0.75 : 0)
