#TIL I COLLAPSE
use_bpm 83
use_synth :piano

M1 = [:cs4, :gs4, :gs4, :gs4, :gs4, :gs4, :fs4, :gs4]
i = 0

live_loop :m do
  
  #M1
  8.times do
    play M1[i]
    sleep 0.5
    i = i + 1
  end
  i = 0
  
  #M2
  play :a4, amp: 1.5
  sleep 0.5
  play :gs4, amp: 1.5
  sleep 3.5
  
  #M3
  8.times do
    play M1[i]
    sleep 0.5
    i = i + 1
  end
  i = 0
  
  #M4
  play :e4, amp: 2
  sleep 3.5
  
  #M5
  8.times do
    play M1[i]
    sleep 0.5
    i = i + 1
  end
  i = 0
  
  #M6
  play :a4, amp: 1.5
  sleep 0.5
  play :gs4, amp: 1.5
  sleep 3.5
  
  #M7
  8.times do
    play M1[i]
    sleep 0.5
    i = i + 1
  end
  i = 0
  #M8
  play :e4, amp: 1
  sleep 4
end

