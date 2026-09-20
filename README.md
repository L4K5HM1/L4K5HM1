# Hi, I'm Lakshmi

I'm a computer science student at UT Austin and a member of ECLAIR's VHA team. I'm learning about software and robotics through coursework and projects.

## My HAND onboarding project

I looked at how to reduce jitter in webcam hand tracking. Starting with the team's MediaPipe demo, I recorded my hand moving and staying still, then compared two exponential moving average (EMA) settings on the index fingertip's X and Y positions.

In the stationary recording, EMA 0.2 reduced average frame-to-frame movement by **51.3%** across 682 frame pairs. EMA 0.7 reduced it by **17.2%**. The stronger setting gave a steadier signal, but the movement graphs showed it taking longer to catch up when my hand moved.

These results come from one stationary recording. They measure how much the reported position changed between frames; they don't establish how close it was to the fingertip's actual position.

[See my notebook, graphs, and recordings](https://github.com/EthanGopez/HAND/tree/vha_onboarding_lmuppana/onboarding/vha/lmuppana)

I used the demo from [ECLAIR's HAND project](https://github.com/EthanGopez/HAND) and had AI help with setup and code. I tested the smoothing on saved recordings and haven't used it to control a physical robot YET.
