# Hi, I'm Lakshmi

I'm a computer science student at UT Austin and part of ECLAIR's VHA team. I'm learning through projects in software and robotics.

## ECLAIR HAND: Fingertip smoothing experiment

For VHA onboarding, I explored how smoothing affects steadiness and responsiveness in webcam hand tracking. Using the team's MediaPipe demo, I recorded hand landmarks and compared two exponential moving average (EMA) settings for the index fingertip.

- Compared original and smoothed X/Y coordinates in movement graphs.
- Tested steadiness across 682 consecutive-frame pairs in a separate stationary-hand recording.
- EMA 0.2 reduced average frame-to-frame movement by **51.3%** in that recording, compared with **17.2%** for EMA 0.7. Stronger smoothing also visibly delayed the response to movement.
- Documented the method, results, and limitations in a notebook. These measurements show reduced movement, not proof of improved tracking accuracy.

[View my notebook and recordings](https://github.com/EthanGopez/HAND/tree/vha_onboarding_lmuppana/onboarding/vha/lmuppana)

Built on the provided demo from [ECLAIR's HAND project](https://github.com/EthanGopez/HAND), with AI assistance during setup, implementation, and documentation. This was an analysis of saved recordings, not a physical robot-control test.
