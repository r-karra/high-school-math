# 📘 TS Intermediate 2B — Mock Questions: Solutions

This file contains detailed solutions for the four mock questions on **Circles**, **Indefinite Integrals**, and **Definite Integrals**.

---

## 🧮 Q1. Circle through two points, center on a line

**Question:**  
Find the equation of a circle that passes through the points (2,3) and (4,5), and whose center lies on the line:

$$
x - y - 1 = 0
$$

---

### ✔ Solution


Let the center be \((h, k)\) and radius be \(r\).

Since the circle passes through \((2,3)\) and \((4,5)\):

$$
(2 - h)^2 + (3 - k)^2 = r^2 \tag{1}
$$

$$
(4 - h)^2 + (5 - k)^2 = r^2 \tag{2}
$$



Subtract (1) from (2):

$$
(4-h)^2 - (2-h)^2 + (5-k)^2 - (3-k)^2 = 0
$$

Using \(a^2 - b^2 = (a-b)(a+b)\):

- For \(x\)-terms:

$$
(4-h)^2 - (2-h)^2 = (2)(6 - 2h) = 12 - 4h
$$

- For \(y\)-terms:

$$
(5-k)^2 - (3-k)^2 = (2)(8 - 2k) = 16 - 4k
$$

So:

$$
(12 - 4h) + (16 - 4k) = 0 \Rightarrow 28 - 4(h + k) = 0
$$

$$
h + k = 7 \tag{3}
$$

Center lies on:

$$
h - k = 1 \tag{4}
$$

Solving (3) & (4):

$$
\begin{cases}
h + k = 7 \\
h - k = 1
\end{cases}
\Rightarrow h = 4,\; k = 3
$$

Now radius using point (2,3):

$$
r^2 = (2-4)^2 + (3-3)^2 = 4 \Rightarrow r = 2
$$

**Final equation:**

$$
(x - 4)^2 + (y - 3)^2 = 4
$$

General form:

$$
x^2 + y^2 - 8x - 6y + 21 = 0
$$

---

## 🧮 Q2. Indefinite Integral — Algebraic Simplification

**Question:**

$$
\int \frac{3x^2 + 4x + 5}{(x+1)^3} \, dx
$$

---

### ✔ Solution

Let:

$$
u = x + 1 \Rightarrow x = u - 1
$$

Then:

$$
3x^2 + 4x + 5 = 3(u-1)^2 + 4(u-1) + 5 = 3u^2 - 2u + 4
$$

So:

$$
\frac{3x^2 + 4x + 5}{(x+1)^3} = \frac{3u^2 - 2u + 4}{u^3}
= \frac{3}{u} - \frac{2}{u^2} + \frac{4}{u^3}
$$

Integrate:

$$
\int \left( \frac{3}{u} - \frac{2}{u^2} + \frac{4}{u^3} \right) du
= 3\ln|u| + \frac{2}{u} - \frac{2}{u^2} + C
$$

Substitute back:

$$
\boxed{3\ln|x+1| + \frac{2}{x+1} - \frac{2}{(x+1)^2} + C}
$$

---

## 🧮 Q3. Circle from a family, tangent to the y-axis

**Question:**

$$
x^2 + y^2 - 4x + 3 = \lambda (x^2 + y^2 - 2x - 3y + 5)
$$

Find the circle that is tangent to the y-axis.

---

### ✔ Solution (Condensed)

Rewrite:

$$
(1-\lambda)(x^2+y^2)+(-4+2\lambda)x+3\lambda y+(3-5\lambda)=0
$$

Convert to standard form:

$$
x^2+y^2+2gx+2fy+c=0
$$

Where:

$$
g = \frac{\lambda - 2}{1-\lambda}, \quad f = \frac{3\lambda}{2(1-\lambda)}
$$

Center:

$$
(h,k) = (-g,-f) = \left(\frac{\lambda - 2}{\lambda - 1}, \frac{3\lambda}{2(\lambda - 1)}\right)
$$

Radius squared:

$$
r^2 = \frac{-7\lambda^2 + 16\lambda + 4}{4(\lambda - 1)^2}
$$

Tangency to y-axis:

$$
|h| = r \Rightarrow h^2 = r^2
$$

Solving:

$$
11\lambda^2 - 32\lambda + 12 = 0
$$

Roots:

$$
\boxed{\lambda = \frac{16 \pm 2\sqrt{31}}{11}}
$$

---

## 🧮 Q4. Definite Integral

**Question:**

$$
\int_0^{\frac{\pi}{2}} \frac{\sin x}{1 + \cos x} \, dx
$$

---

### ✔ Solution

Let:

$$
u = 1 + \cos x \Rightarrow du = -\sin x\,dx
$$

Limits:

- \(x=0 \Rightarrow u=2\)
- \(x=\frac{\pi}{2} \Rightarrow u=1\)

So:

$$
-\int_{2}^{1} \frac{1}{u} du = \ln 2
$$

**Final answer:**

$$
\boxed{\ln 2}
$$

---

_End of solutions._
