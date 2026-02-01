---
author: rc
class: note
tags:
description:
source:
related:
date created: 2026-02-10T15:27:22
last update: 1970-01-29T00:00:01
aliases:
  - PID
---


Proportional-Integral-Derivative or PID controllers are a feedback control loops. %%odd wording :/%%


![[PID_Flow.png]] Figure: Wikipedia ([Link](https://en.wikipedia.org/wiki/Proportional%E2%80%93integral%E2%80%93derivative_controller))


A PID controller starts at the input $r(t)$ (aka: reference, setpoint, SP). Where $r(t)$ is used to generate the error signal $e(t)$ (aka: process variable, PV) by subtracting the output $y(t)$ (feedback).

$$e(t)=r(t)-y(t)$$


# Proportional the P Term
The P term is the error signal $e(t)$ proportionately set with a gain factor $K_{p}$.

$$p(t)=K_{p} e(t)= K_{p}(r(t)-y(t))$$


# Integral the I Term



# Derivative the D Term
