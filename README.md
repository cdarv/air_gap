# AIR GAP

> *"The only safe network is the one nothing touches."*

A cybersecurity roguelite that fits in [one HTML file](index.html). Twin-stick defense of a bioluminescent network, where every monster is a real attack and every tool is a real defense — and the wrong tool simply **does not work**. No quizzes, no lectures. The lessons arrive the moment you feel them.

**[▶ PLAY — github.io/…/air_gap](https://cdarv.github.io/air_gap/)** · single file, no install, desktop (WASD + mouse)

## What you actually play

You are one program — a lantern in a dark network of glowing nodes. Waves of attack arrive with visible telltales:

| Threat | Real concept | What actually stops it |
|---|---|---|
| The swarm | DDoS (availability) | **Rate-Limit** — volume is answered by policy |
| The worm | Ransomware (integrity) | **Encrypt** — guard what is owned; it converts nodes |
| The spoof | Phishing (confidentiality) | **Deep Scan** — it wears friendly colors; you cannot fight what you cannot distinguish |

Fire at the wrong thing and your shot *bounces with a sad thud* and a one-line reason. That bounce is the tutorial. The curriculum is the CIA triad, and you learn it the way defenders do — by having the wrong tool in hand when it matters.

**Focus (hold RMB)** slows time so *you* — not automation — tag what looks legitimate. Automation handles scale; humans catch what looks normal. That sentence is a verb in this game.

## Structure (this POC is a full vertical slice)

- **Fail-safe cold open** — a scripted first cluster that is Cybersecurity 101 disguised as an easy level
- **Roguelite runs** — random clusters, pick-1-of-3 upgrade cards where every card is a real defense mechanism (Salting, Honeypot Node, Zero Trust, MFA Gate, Backups…), choose-your-path map with partial intel
- **A zero-day boss** — immune until you scan it twice. You cannot fight what you cannot see.
- **Deaths are curriculum** — every death names what killed you and why your counter failed, and grants a permanent "+lessons learned" edge
- **An intel codex** — entries unlock on first contact; 17 concepts, zero gating
- **THE FLIP** — win the run and the story turns: thirty seconds as the malware, eating the network you just defended. *Act II — The Red Lantern — to be continued.*

## Act II roadmap

Replay the siege from the attacker's side: MITM shadows, a brute-force golem, an SQL-injection puppet, and a rootkit that **rewrites your debriefs to lie to you.**

## Build notes

- One file. Three.js from cdnjs. No assets, no build step — every sound is synthesized in WebAudio (swarm proximity crackle, the wet locking of a worm encrypting a node, wrong-tool thud).
- Progress (codex, lessons, wins) lives in `localStorage`.

Made in one session because someone wanted to learn cybersec by *shooting it*.
