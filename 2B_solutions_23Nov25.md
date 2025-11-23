# 📘 TS Intermediate 2B — Mock Questions: Solutions

This file contains detailed solutions for the four mock questions on **Circles**, **Indefinite Integrals**, and **Definite Integrals**.

---

## 🧮 Q1. Circle through two points, center on a line

**Question:**  
Find the equation of a circle that passes through the points \((2,3)\) and \((4,5)\), and whose center lies on the line
\[
 x - y - 1 = 0.
\]

---

### ✅ Solution
Let the center of the circle be \((h, k)\) and radius be \(r\).

Since the circle passes through \((2,3)\) and \((4,5)\):
\[
(2 - h)^2 + (3 - k)^2 = r^2 \quad\text{(1)}
\]
\[
(4 - h)^2 + (5 - k)^2 = r^2 \quad\text{(2)}
\]
Subtract (1) from (2):
\[
(4 - h)^2 - (2 - h)^2 + (5 - k)^2 - (3 - k)^2 = 0.
\]
Use the identity \(a^2 - b^2 = (a-b)(a+b)\):

- For the \(x\)-terms:
  \[
  (4-h)^2 - (2-h)^2 = (2)(6 - 2h) = 12 - 4h.
  \]
- For the \(y\)-terms:
  \[
  (5-k)^2 - (3-k)^2 = (2)(8 - 2k) = 16 - 4k.
  \]
So:
\[
(12 - 4h) + (16 - 4k) = 0
\Rightarrow 28 - 4(h + k) = 0
\Rightarrow h + k = 7. \quad\text{(3)}
\]

The center \((h, k)\) lies on the line \(x - y - 1 = 0\), so:
\[
 h - k - 1 = 0 \Rightarrow h - k = 1. \quad\text{(4)}
\]
Solve (3) and (4):
\[
\begin{cases}
 h + k = 7 \\
 h - k = 1
\end{cases}
\Rightarrow 2h = 8 \Rightarrow h = 4,
\]
then \(k = 7 - 4 = 3\).

So the center is \((4,3)\).

Now find the radius using point \((2,3)\):
\[
 r^2 = (2 - 4)^2 + (3 - 3)^2 = (-2)^2 + 0 = 4
\Rightarrow r = 2.
\]

Hence the equation of the circle is:
\[
 (x - 4)^2 + (y - 3)^2 = 4.
\]
In general form:
\[
 x^2 + y^2 - 8x - 6y + 21 = 0.
\]

---

## 🧮 Q2. Indefinite integral with algebraic simplification

**Question:**  
Evaluate:
\[
 \int \frac{3x^2 + 4x + 5}{(x+1)^3} \, dx.
\]

---

### ✅ Solution
Let
\[
 u = x + 1 \Rightarrow x = u - 1.
\]
Then
\[
 3x^2 + 4x + 5 = 3(u-1)^2 + 4(u-1) + 5.
\]
Expand:
\[
3(u^2 - 2u + 1) + 4u - 4 + 5 = 3u^2 - 6u + 3 + 4u + 1 = 3u^2 - 2u + 4.
\]
So the integrand becomes:
\[
\frac{3x^2 + 4x + 5}{(x+1)^3} = \frac{3u^2 - 2u + 4}{u^3} = \frac{3}{u} - \frac{2}{u^2} + \frac{4}{u^3}.
\]
Thus,
\[
 \int \frac{3x^2 + 4x + 5}{(x+1)^3} \, dx = \int \left(\frac{3}{u} - \frac{2}{u^2} + \frac{4}{u^3}\right) du.
\]
Integrate term by term:
\[
 \int \frac{3}{u} \, du = 3 \ln|u|,
\]
\[
 \int -\frac{2}{u^2} \, du = -2 \int u^{-2} du = -2 \left( \frac{u^{-1}}{-1} \right) = \frac{2}{u},
\]
\[
 \int \frac{4}{u^3} \, du = 4 \int u^{-3} du = 4 \left( \frac{u^{-2}}{-2} \right) = -\frac{2}{u^2}.
\]
So the final result is:
\[
 3 \ln|u| + \frac{2}{u} - \frac{2}{u^2} + C.
\]
Substitute back \(u = x+1\):
\[
 \boxed{\int \frac{3x^2 + 4x + 5}{(x+1)^3} \, dx = 3 \ln|x+1| + \frac{2}{x+1} - \frac{2}{(x+1)^2} + C}.
\]

---

## 🧮 Q3. Circle from a family, tangent to the y-axis

**Question:**  
From the family of circles
\[
 x^2 + y^2 - 4x + 3 = \lambda (x^2 + y^2 - 2x - 3y + 5),
\]
find the circle(s) that are **tangent to the y-axis**.

---

### ✅ Solution (Outline + Key Results)

First, rewrite the family in standard circle form.

Bring all terms to one side:
\[
 x^2 + y^2 - 4x + 3 - \lambda(x^2 + y^2 - 2x - 3y + 5) = 0.
\]
Expand and group:
\[
 (1-\lambda)(x^2 + y^2) + (-4 + 2\lambda)x + 3\lambda y + (3 - 5\lambda) = 0.
\]
Assume \(\lambda \neq 1\), and divide by \((1-\lambda)\) to write in the form
\[
 x^2 + y^2 + 2gx + 2fy + c = 0.
\]
Then
\[
 2g = \frac{-4 + 2\lambda}{1-\lambda}, \quad 2f = \frac{3\lambda}{1-\lambda}, \quad c = \frac{3 - 5\lambda}{1-\lambda}.
\]
So,
\[
 g = \frac{\lambda - 2}{1-\lambda}, \quad f = \frac{3\lambda}{2(1-\lambda)}.
\]
The center \((h,k)\) is \((-g, -f)\):
\[
 h = -g = \frac{\lambda - 2}{\lambda - 1}, \quad k = -f = \frac{3\lambda}{2(\lambda - 1)}.
\]
The radius squared is
\[
 r^2 = g^2 + f^2 - c,
\]
which simplifies to
\[
 r^2 = \frac{-7\lambda^2 + 16\lambda + 4}{4(\lambda - 1)^2}.
\]

For the circle to be **tangent to the y-axis** (line \(x = 0\)), the distance from the center to the y-axis must equal the radius:
\[
 |h| = r \quad \Rightarrow \quad h^2 = r^2.
\]
So,
\[
 \left(\frac{\lambda - 2}{\lambda - 1}\right)^2 = \frac{-7\lambda^2 + 16\lambda + 4}{4(\lambda - 1)^2}.
\]
Multiply both sides by \(4(\lambda - 1)^2\):
\[
 4(\lambda - 2)^2 = -7\lambda^2 + 16\lambda + 4.
\]
Expand:
\[
 4(\lambda^2 - 4\lambda + 4) = -7\lambda^2 + 16\lambda + 4,
\]
\[
 4\lambda^2 - 16\lambda + 16 = -7\lambda^2 + 16\lambda + 4.
\]
Bring all terms to one side:
\[
 4\lambda^2 - 16\lambda + 16 + 7\lambda^2 - 16\lambda - 4 = 0,
\]
\[
 11\lambda^2 - 32\lambda + 12 = 0.
\]
Solve the quadratic:
\[
 \lambda = \frac{32 \pm \sqrt{32^2 - 4\cdot 11 \cdot 12}}{2\cdot 11} = \frac{32 \pm \sqrt{1024 - 528}}{22} = \frac{32 \pm \sqrt{496}}{22} = \frac{32 \pm 4\sqrt{31}}{22} = \frac{16 \pm 2\sqrt{31}}{11}.
\]

So there are **two** values of \(\lambda\):
\[
 \lambda_1 = \frac{16 - 2\sqrt{31}}{11}, \quad \lambda_2 = \frac{16 + 2\sqrt{31}}{11}.
\]
Each gives a circle from the family which is tangent to the y-axis.

Substituting back into the family equation and simplifying, the two tangent circles can be written (after clearing denominators) as:

1. For \(\lambda_1 = \dfrac{16 - 2\sqrt{31}}{11}\):
\[
 (5 - 2\sqrt{31})(x^2 + y^2) + (12 + 4\sqrt{31})x + (6\sqrt{31} - 48)y + (47 - 10\sqrt{31}) = 0.
\]

2. For \(\lambda_2 = \dfrac{16 + 2\sqrt{31}}{11}\):
\[
 (5 + 2\sqrt{31})(x^2 + y^2) + (12 - 4\sqrt{31})x - (48 + 6\sqrt{31})y + (47 + 10\sqrt{31}) = 0.
\]

Either form with \(\lambda\) substituted back into the original family is acceptable; the key ideas are:
- expressing center and radius in terms of \(\lambda\),
- applying the tangency condition \(|h| = r\),
- solving for \(\lambda\).

---

## 🧮 Q4. Definite integral with trigonometric manipulation

**Question:**  
Evaluate:
\[
 \int_0^{\frac{\pi}{2}} \frac{\sin x}{1 + \cos x} \, dx.
\]

---

### ✅ Solution
Use the substitution:
\[
 u = 1 + \cos x \Rightarrow du = -\sin x \, dx.
\]
Then
\[
 \sin x \, dx = -du,
\]
and the integral becomes
\[
 \int_0^{\frac{\pi}{2}} \frac{\sin x}{1 + \cos x} \, dx = -\int_{u(0)}^{u(\pi/2)} \frac{1}{u} \, du.
\]
Compute the new limits:
\[
 x = 0 \Rightarrow u = 1 + \cos 0 = 1 + 1 = 2,
\]
\[
 x = \frac{\pi}{2} \Rightarrow u = 1 + \cos \frac{\pi}{2} = 1 + 0 = 1.
\]
So
\[
 -\int_{2}^{1} \frac{1}{u} \, du = -\left[\ln|u|\right]_{2}^{1} = -\big(\ln 1 - \ln 2\big) = -\big(0 - \ln 2\big) = \ln 2.
\]

Therefore,
\[
 \boxed{\int_0^{\frac{\pi}{2}} \frac{\sin x}{1 + \cos x} \, dx = \ln 2.}
\]

An alternative method (also valid in exams) is to multiply numerator and denominator by \(1 - \cos x\) and use trigonometric identities.

---

End of **solutions.md** — you can pair this with `questions.md` in a GitHub repo for a neat practice set.

