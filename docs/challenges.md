# Challenges

Hard problems met while building TriBot Music, and what fixed them. Back to the [README](../README.md).

## Beat trackers file songs at the wrong tempo

**Problem.** Every transition depends on the beat grid. **What went wrong.** Some songs were filed at a related tempo, 4:3 or 3:2 off, or at double. A song's real drum pattern repeated every few seconds against a grid that disagreed, so anything laid on the beat sounded off. Listeners heard a pad routine that was "so off beat". **What fixed it.** A tempo check with three witnesses: how often the bars repeat, the published tempo where one exists, and how well the drum stem fits a straight grid. A song is re-filed when two agree. New songs go through it as they are learned.

## Two singers colliding

**Problem.** Listeners heard artists cut off mid-sentence, starting mid-sentence, or talking over each other. **What went wrong.** Moves were timed to the beat, not the lyric. **What fixed it.** Word-level lyric alignment gave each singer's lines exact spans. "Line to line" became the base of every transition. Then a rule: no two singers at once outside a few deliberate overlap moves, with a final pass on every move that removes any collision, a pitch shift of at most half a semitone with a return to true pitch, and an echo-out fallback.

## The same synth on every transition

**Problem.** The owner said the added instruments sounded artificial and boring, the same on every track. **What went wrong.** The riser, impact and chord sounds were synthesised the same way each time. **What fixed it.** Sounds are now picked per transition from the records first, then a genre instrument, then a generated sound, and never repeat the last transition's. A trial on real songs then caught follow-up faults. The chords were meant to be chopped from the record but never were: a chop was only allowed where nobody sings, and on real songs someone sings or raps in nearly every half bar. The rule now allows a chop under light singing, since the chop is cut from the separated music and not the full mix. A made riser was much quieter than the recorded one it stood in for, and is now matched to its loudness. The same trial found the punchy bass was cut short and left silence between far-apart kicks, fixed by letting the note hold.

## A redrum whose low end vanished

**Problem.** Between kicks the redrum had almost no bass. **What went wrong.** With the outgoing bassline muted and the loop filtered away, the DJ's kick was a short thud with nothing under it. **What fixed it.** Each kick's low end is now held until the next, and a beat emptied on purpose before the drop is no longer read as a hole.

## One GPU, a live set and background learning

**Problem.** A live set must never wait, yet learning songs uses the same GPU. **What went wrong.** At one point an AI call ran inline on the planning path and a set stopped after one song. **What fixed it.** A priority lock: live work first, everything else in small pieces that step aside. Slow work is cached or run in the background.

## Keeping generated audio on the beat

**Problem.** Generated mixes showed distortion on some instruments. **What went wrong.** Re-timing a take that was already on the beat bent its notes, which sounded like a tone shift mid-note. **What fixed it.** A take already on the beat is left alone, and re-timing never bends the notes.
