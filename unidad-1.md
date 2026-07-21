setcpm(100) // 140 beat

const PIANO_ON   = 1
const PIANO_ON2  = 1

$piano : note("{<[b4 g4 e4] [b4 g4 e4] [a4 0 f#4] [0 0 d#4 e4 f#4 0 0] [b4 g4 e4] [b4 g4 e4] [c5 0 b4] [0 a4 0]>}")
  .sound("piano")  
  .postgain(PIANO_ON ? 0.5 : 0)

$piano : note("{<[[e3] [[e3, g3, b3] [e3, g3, b3]]] [[b2] [eb3, f#3, a3] [eb3, f#3, a3]] [[e3] [e3, g3, b3] [e3, g3, b3]] [[a] [eb, a, c] [eb3, f#3, a3]]>}")
  .sound("piano")  
  .postgain(PIANO_ON2 ? 0.5 : 0)
