---
author: rc
class: example
tags:
description:
source: https://www.youtube.com/watch?v=bz7P2ROXYMw
related:
date created: 2026-02-01T16:31:00
last update: 2026-02-01T17:23:00
aliases:
---
![[0x001 - RLC Transfer Function Example Figure 1.png]]
![[0x001 - RLC Transfer Function Example Figure 2.png]]

Say the goal is to find $\frac{V_{c}(s)}{V(s)}$. Where $V_{c}(s)$ is the voltage across the capacitor and $V(s)$ is the input voltage.

First we need some equations. Using [[Kirchhoff's Voltage Law|KVL]] to find the equations of the two loops.

The left loop (1):
$$V(s)=R_{1}I_{1}(s)+Ls(I_{1}(s)-I_{2}(s))$$

$$V(s)=(R_{1}+Ls)I_{1}(s)-LsI_{2}(s)$$

The right loop (2):
$$0=R_{2}I_{2}(s)+\frac{1}{Cs}I_{2}(s)+Ls(I_2(s)-I_{1}(s))$$

$$0=(R_{2}+\frac{1}{Cs}+Ls)I_{2}(s)-LsI_{1}(s)$$

Here lets prepare to substitute $I_{1}(s)$ this will leave $I_{2}(s)$ which using $V_{c}(s)=\frac{1}{Cs}I_{2}(s)$ we can find $\frac{V_{c}(s)}{V(s)}$.


(2)
$$I_{1}(s)=\left( \frac{R_{2}}{Ls}+\frac{1}{LCs^2}+1 \right)I_{2}(s)$$

now putting (2)->(1)

$$V(s)=(R_{1}+Ls)\left( \frac{R_{2}}{Ls}+\frac{1}{LCs^2}+1 \right)I_{2}(s)-LsI_{2}(s)$$

$$\frac{V(s)}{I_{2}(s)}=(R_{1}+Ls)\left( \frac{R_{2}}{Ls}+\frac{1}{LCs^2}+1 \right)-Ls$$

$$\frac{V(s)}{I_{2}(s)}=\frac{(R_{1}+Ls)\left(R_{2}Cs+1+LCs^2 \right)-L^2Cs^3 }{LCs^2}$$

$$\frac{I_{2}(s)}{V(s)}=\frac{LCs^2}{(R_{1}+Ls)\left(R_{2}Cs+1+LCs^2 \right)-L^2Cs^3 }$$
expand
$$\frac{I_{2}(s)}{V(s)}=\frac{LCs^2}{R_{1}LCs^2+L^2Cs^3+R_{1}+Ls+R_{1}R_{2}Cs+R_{2}LCs^2-L^2Cs^3 }$$

$$\frac{I_{2}(s)}{V(s)}=\frac{LCs^2}{(R_{1}+R_{2})LCs^2+(L+R_{1}R_{2}C)s+R_{1}}$$

Now with $V_{c}(s)=\frac{1}{Cs}I_{2}(s)$.

$$V_{c}(s)Cs=I_{2}(s)$$

$$\frac{V_{c}(s)Cs}{V(s)}=\frac{LCs^2}{(R_{1}+R_{2})LCs^2+(L+R_{1}R_{2}C)s+R_{1}}$$

$$\boxed{\frac{V_{c}(s)}{V(s)}=\frac{Ls}{(R_{1}+R_{2})LCs^2+(L+R_{1}R_{2}C)s+R_{1}}}$$
