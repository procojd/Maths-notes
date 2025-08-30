# Fourier Series: Beginner to Intermediate Guide

## 1. Introduction

The **Fourier Series** is a powerful mathematical tool that allows us to represent **periodic functions** as a sum of simple **sine and cosine waves**.  
This idea was introduced by **Joseph Fourier** in the early 19th century and has since become a foundation of signal processing, physics, and engineering.

https://www.instagram.com/reel/DKcRYvHx9Mb/?utm_source=ig_web_copy_link

A periodic function can be written as an **infinite trigonometric series**.  

---

## 2. What is a Periodic Function?

A function \( f(x) \) is **periodic** if it repeats its values in equal intervals of length \( T \).

\[
f(x + T) = f(x) \quad \forall x
\]

- \( T \) → period of the function  
- Example: \( \sin(x) \) and \( \cos(x) \) are periodic with period \( 2\pi \).

---

## 3. General Form of Fourier Series

For a periodic function \( f(x) \) with period \( 2L \), the Fourier series expansion is:

\[
f(x) = a_0 + \sum_{n=1}^{\infty} \Big[ a_n \cos\left(\frac{n\pi x}{L}\right) + b_n \sin\left(\frac{n\pi x}{L}\right) \Big]
\]

Where coefficients are defined as:

\[
a_0 = \frac{1}{2L} \int_{-L}^{L} f(x)\, dx
\]

\[
a_n = \frac{1}{L} \int_{-L}^{L} f(x)\cos\left(\frac{n\pi x}{L}\right)\, dx
\]

\[
b_n = \frac{1}{L} \int_{-L}^{L} f(x)\sin\left(\frac{n\pi x}{L}\right)\, dx
\]

---

## 4. Key Ideas

- **\( a_0 \)** → average/constant term of the function.  
- **\( a_n \cos \)** → captures even (symmetric) parts of the function.  
- **\( b_n \sin \)** → captures odd (antisymmetric) parts of the function.  
- Adding more terms → gives a better approximation of \( f(x) \).

---

## 5. Example 1: Square Wave

Consider a square wave of period \( 2\pi \):

\[
f(x) = \begin{cases} 
1 & 0 < x < \pi \\
-1 & -\pi < x < 0 
\end{cases}
\]

Fourier expansion:

\[
f(x) = \frac{4}{\pi} \Big( \sin(x) + \frac{1}{3}\sin(3x) + \frac{1}{5}\sin(5x) + \cdots \Big)
\]

👉 Only **odd sine terms** appear because the square wave is **odd symmetric**.

---

## 6. Example 2: Sawtooth Wave

For \( f(x) = x \) on \( (-\pi, \pi) \), Fourier series is:

\[
f(x) = 2 \Big( -\sin(x) - \frac{1}{2}\sin(2x) - \frac{1}{3}\sin(3x) - \cdots \Big)
\]

---

## 7. Convergence of Fourier Series

- Fourier series converges to \( f(x) \) at all **points of continuity**.  
- At points of **discontinuity**, it converges to the **average of left and right limits** (Gibbs phenomenon).  

---

## 8. Applications of Fourier Series

- **Signal processing**: Breaking down signals into frequencies.  
- **Electrical engineering**: Analyzing AC waveforms.  
- **Physics**: Heat conduction (original motivation by Fourier).  
- **Audio processing**: Sound waves are decomposed into frequencies.  
- **Image compression**: Basis for JPEG and other transforms.  

---

## 9. Complex Form of Fourier Series

Instead of sines and cosines, we can use **complex exponentials** via Euler’s formula:

\[
f(x) = \sum_{n=-\infty}^{\infty} c_n e^{i n \pi x / L}
\]

Where:

\[
c_n = \frac{1}{2L} \int_{-L}^{L} f(x) e^{-i n \pi x / L} \, dx
\]

This form is widely used in **engineering and physics** because it connects naturally to the **Fourier Transform**.

---

## 10. Summary

- Fourier series represents periodic functions as sums of sine and cosine terms.  
- Coefficients \( a_n, b_n \) are calculated by integration.  
- Square, sawtooth, and triangle waves are classic examples.  
- Convergence depends on continuity and smoothness.  
- Complex form is more elegant and leads to Fourier Transform.  

---
