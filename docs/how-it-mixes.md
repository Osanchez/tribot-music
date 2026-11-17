# How it mixes

How the DJ decides and performs a transition, for a reader who knows music but not the code. Back to the [README](../README.md).

## Picking the next song

Listener requests go first. Otherwise the DJ looks for songs it already knows that fit the one playing in key and tempo, weighs them by genre, energy, where the night is, how cleanly the singers can hand over and what is charting, and draws one. The full process, including how the pair is matched and the move chosen, is in [how it chooses](how-it-chooses.md).

## The night's arc

A set warms up for a couple of songs, builds over three, holds a peak for three, gives the room one breather, and goes round again. Each phase aims at a share of the library's own energy range, so it works with whatever the library holds. The extras follow the phase: a pump and a riser into a peak, nothing over a breather.

## The moves

| Move | What happens |
|---|---|
| Stem blend | The next song comes in piece by piece: hats, then drums, then bass on the downbeat, then the voice. |
| Line to line | The base layer of every transition, not a move of its own. Each singer is heard in whole lines: the outgoing singer finishes a line, the next comes in on theirs. |
| Redrum | The DJ's own drum kit plays the next song's beat over a loop of the outgoing song, then drops into the next song. It ends one of six ways: a roll, an echo, a spinback, a tape stop, a filter close or a pull. Never the same ending twice running. |
| Pad routine | The outgoing song is chopped and retriggered on pads like an MPC performance, with the DJ's own instruments (chords, bass, lead, kick) played in the song's key over it. |
| Echo out | The last word echoes away, then the next song starts. Works for any two songs and is the usual fallback. |
| Quick cut | A clean skip. The last resort. |
| Scratch | The next song's first beat is scratched over the outgoing instrumental, then dropped in clean. |
| Drum bridge | A drum loop carries the join into a next song whose intro has no drums. |
| Carry over | For a singer who never pauses: the stem blend, a way out, a quick cut or a redrum is chosen by ear for where the voice can safely hand over. |
| Extras | A riser, a crash, a pump and a landing kick, each with its own switch in Settings. |

The core moves are on by default. Several experimental ones, such as a lyric loop on a shared word, are off until switched on, and earn their place on votes.

## The rules it never breaks

- **On the beat.** Anything laid over a song sits on that song's tracked beats, and locks to its kick pattern. It is never spaced by a fixed tempo figure.
- **One singer at a time.** The planner keeps two lead vocals apart, with a final check on every move. A few moves that overlap voices on purpose are the stated exceptions.
- **The last word is never cut.** An outgoing singer is not stopped mid-decay. They finish the line, or the word is echoed out at its end.
- **Small pitch moves only.** A next singer brought in over another band may be tuned by at most half a semitone, and returns to true pitch by the downbeat.
- **One low end at a time.** Two basslines, or two drummers, are not left fighting under a singer.
- **The live set is never blocked or slowed.** If a transition cannot be made in time, a simpler one plays.

## Sounds picked per transition

Added in November 2026. The chords, bass, risers, swells and impacts the DJ adds are chosen from the two songs' genre, key fit, tempo and energy, and from the night. The order of preference:

1. The records first: a chord stab chopped from the song's own music, a swell made from the next song's first downbeat.
2. Then an instrument of the genre.
3. A generated sound last.

It is never the same as the last transition's, and planning the same transition again picks the same sounds.

## Explaining itself

Each transition keeps the reasons for its choices: why that move, which singer leaves where, which sounds. The panel shows them next to the rating buttons.
