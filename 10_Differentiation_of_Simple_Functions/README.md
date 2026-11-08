---
tags:
    - Differentiation
    - Limits
    - Derivatives
    - Differentiation Rules
    - Chain Rule
    - Product Rule
    - Quotient Rule
    - Power Rule
    - Exponential Functions
    - Logarithmic Functions
    - Tangent Lines
    - Velocity
    - Acceleration
---

<h1 align="center">Differentiation of Simple Functions</h1>

In this session, we introduce differentiation and its fundamental role in mathematical analysis and software development. We begin with the derivative and its geometric meaning as the slope of the tangent line, which is essential for optimisation problems and algorithm analysis.

The session covers differentiation rules including the chain, product, and quotient rules, as well as derivatives of exponential and logarithmic functions. The exercises move from limits and basic derivatives to more advanced rules and applications such as velocity and acceleration. Special emphasis is placed on how differentiation supports machine learning, optimisation, and numerical methods.

#### Key Concepts

- Limits and the derivative as rate of change
- Differentiation rules: power, product, quotient, and chain rules
- Derivatives of exponential and logarithmic functions
- Applications to motion and optimisation

!!! tip "Learning Objectives"

    - Evaluate limits and interpret the derivative geometrically.
    - Differentiate functions using standard rules.
    - Apply the product, quotient, and chain rules correctly.
    - Find derivatives of exponential and logarithmic functions.
    - Use differentiation to analyse velocity, acceleration, and rates of change.

<hr/>

### Session Preparation

[Chapter 10](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/RBrooksDK/MSE_book_v2/main/main.pdf) (English)<br>
[Kapitel 10](https://docs.google.com/viewer?url=https://raw.githubusercontent.com/RBrooksDK/MSE_book_v2_da/main/main.pdf) (Dansk)

Some of the exercises may require you to use Python. You may also need to install the `numpy` and `sympy` libraries if you haven't already.

### Resources

[Session Resources](https://viaucdk-my.sharepoint.com/:f:/g/personal/frbj_viauc_dk/IgDnkFsvBsyqQLOHBETOgY1IAQlXM2CikHH4SRRyMzUkjaY?e=hVDmVm)

<hr/>

### Exercises

**[Python]** Means that you are advised to use Python to solve the exercise. You can find the Python solutions [here](https://github.com/RBrooksDK/MSE1_26/blob/main/10_Differentiation_of_Simple_Functions/Python_solutions_for_exercises_10.ipynb) or download them [here](Python_solutions_for_exercises_10.ipynb)

#### Exercise 1 (Recap)

**[Python]** Given

$A=\left[\begin{array}{ccc}1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9\end{array}\right]$ and $B=\left[\begin{array}{ccc}9 & 8 & 7 \\ 6 & 5 & 4 \\ 3 & 2 & 1\end{array}\right]$.

Solve the matrix equation $X-A=6(X+B)$.

??? answer "&nbsp;"

    $X=\left[\begin{array}{ccc}-11 & -10 & -9 \\ -8 & -7 & -6 \\ -5 & -4 & -3\end{array}\right]$


#### Exercise 2

Find the limits of the following functions:

1. \(\lim\limits_{x \to 0} \frac{x^4-4 x^3+x^2}{x^3+x^2+x}\)
2. \(\lim\limits_{x \to \infty} \frac{x^2+1}{x^2-1}\)
3. \(\lim\limits_{x \to 2} \frac{x-2}{x^2-3 x+2}\)

??? answer "&nbsp;"

    1. \(\lim\limits_{x \to 0} \frac{x^4-4 x^3+x^2}{x^3+x^2+x} = 0\)
    2. \(\lim\limits_{x \to \infty} \frac{x^2+1}{x^2-1} = 1\)
    3. \(\lim\limits_{x \to 2} \frac{x-2}{x^2-3 x+2} = 1\)

#### Exercise 3: Simple Derivatives

Find the derivatives of the following functions:

1. \(f(x)=x^4\)
2. \(f(t)=t^{-\frac{1}{3}}\)
3. \(y=t^{-3.8}\)

??? answer "&nbsp;"

    1. \(f'(x)=4x^3\)
    2. \(f'(t)=-\frac{1}{3}t^{-\frac{4}{3}}\)
    3. \(y'=-3.8t^{-4.8}\)

#### Exercise 4: Derivatives of Powers
Express the following as powers and then differentiate:

1. \(\frac{1}{x^2}\)
2. \(\sqrt[3]{x}\)
3. \(\frac{1}{x \sqrt[4]{x}}\)

??? answer "&nbsp;"

    1. \(\frac{1}{x^2} = x^{-2}\), derivative: \(\frac{d}{dx}x^{-2} = -2x^{-3}\)
    2. \(\sqrt[3]{x} = x^{1/3}\), derivative: \(\frac{d}{dx}x^{1/3} = \frac{1}{3}x^{-2/3}\)
    3. \(\frac{1}{x \sqrt[4]{x}} = x^{-5/4}\), derivative: \(\frac{d}{dx}x^{-5/4} = -\frac{5}{4}x^{-9/4}\)

#### Exercise 5: Derivatives of Sums and Differences

Find the derivatives of the following functions:

1. \(y=2 x^{-7}+\frac{3}{x^2}\)
2. \(f(u)=u^{\frac{5}{3}}-3 u^{-7}\)
3. \(g(z)=8 z^{-2}-\frac{5}{z}\)

??? answer "&nbsp;"

    1. \(\frac{d}{dx}(2 x^{-7}+\frac{3}{x^2}) = -14x^{-8} - 6x^{-3}\)
    2. \(\frac{d}{dx}(u^{\frac{5}{3}}-3 u^{-7}) = \frac{5}{3}u^{2/3} + 21u^{-8}\)
    3. \(\frac{d}{dx}(8 z^{-2}-\frac{5}{z}) = -16z^{-3} + \frac{5}{z^2}\)

#### Exercises 6: Derivatives of Products and Quotients
Use the product rule to differentiate the functions below:  

1. \(f(x)=\left(4 x^3+2\right)(1-3 x)\)
2. \(g(x)=\left(x^2+x+2\right)\left(x^2+1\right)\)
3. \(h(x)=\frac{x^2-1}{x^3+4}\)
4. \(g(t)=\frac{t(t+6)}{t^2+3 t+1}\)

??? answer "&nbsp;"

    1. \(-48x^3 + 12x^2 - 6\)
    2. \( 4x^3 + 3x^2 + 6x + 1\)
    3. \(h^{\prime}(x)=\frac{-x^4+3 x^2+8 x}{\left(x^3+4\right)^2}\)
    4. \(\frac{-3 t^2+2 t+6}{\left(t^2+3 t+1\right)^2}\)


#### Exercise 7: Derivatives using the Chain Rule
1. \((2 x+3)^2\)
2. \(\left(x^2+2 x+1\right)^{12}\)
3. \(f(t)=\sqrt{t^2-5 t+7}\)
4. \(z=\left(x+\frac{1}{x}\right)^{\frac{3}{7}}\)
5. \(\frac{x}{\sqrt{1-x^2}}\)

??? answer "&nbsp;"

    1. \(8 x+12\)
    2. \(12(2 x+2)\left(x^2+2 x+1\right)^{11}\)
    3. \(\frac{2 t-5}{2 \sqrt{t^2-5 t+7}}\)
    4. \(\frac{3}{7}\left(x+\frac{1}{x}\right)^{-4 / 7}\left(1-\frac{1}{x^2}\right)\)
    5. \(\frac{1}{\left(1-x^2\right)^{3 / 2}}\)

#### Exercise 8: Derivatives of Exponential and Logarithmic Functions

1. \(f(x)=\ln \left(2 x^3\right)\)
2. \(f(x)=e^{x^2+x^3}\)
3. \(f(x)=\ln \left(e^x+x^3\right)\)

??? answer "&nbsp;"

    1. \(\frac{3}{x}\)
    2. \(e^{x^2+x^3} (2x+3x^2)\)
    3. \(\frac{e^x+3x^2}{e^x+x^3}\)

#### Exercise 9: Applications of Derivatives

Velocity is the rate of change of position with respect to time. 

Acceleration is the rate of change of velocity with respect to time.

1. Given the position function of a car $s(t) = 5t^2 + 2t + 1$, where $t$ is in seconds and $s(t)$ is in meters, find the velocity function.

    ??? answer "&nbsp;"

        Velocity function: $v(t) = 10t + 2$ m/s        

2. Knowing that acceleration is the derivative of velocity, find the acceleration function.

    ??? answer "&nbsp;"

        Acceleration function: $a(t) = 10$ m/s²

3. Calculate the velocity and acceleration of the car at $t = 3$ seconds.

    ??? answer "&nbsp;"

        Velocity at $t = 3$ seconds: $v(3) = 32$ m/s

        Acceleration at $t = 3$ seconds: $a(3) = 10$ m/s²

### Challenge Exercises

#### Challenge Exercise 1: Combining Differentiation Rules

Given the function

\(
f(x)=\frac{x^2\sqrt{3x+1}}{(x-2)^3}.
\)

1. Determine the domain of the function.

    ??? answer "&nbsp;"

        \(
        D_f=\left[-\frac13,\infty\right)\setminus\{2\}.
        \)

2. Determine the range of the function. Hint: What values does the function approach as \(x\) approaches the boundaries of its domain?

    ??? answer "&nbsp;"

        \(
        V_f=\mathbb{R}.
        \)

3. Find \(f'(x)\).

    ??? answer "&nbsp;"

        \(
        f'(x)
        =
        \frac{
        \left(
        2x\sqrt{3x+1}
        +
        \frac{3x^2}{2\sqrt{3x+1}}
        \right)(x-2)^3
        -
        3x^2\sqrt{3x+1}(x-2)^2
        }
        {(x-2)^6}.
        \)

        An equivalent simplified form is

        \(
        f'(x)
        =
        \frac{
        \left(
        2x\sqrt{3x+1}
        +
        \frac{3x^2}{2\sqrt{3x+1}}
        \right)(x-2)
        -
        3x^2\sqrt{3x+1}
        }
        {(x-2)^4}.
        \)

4. Calculate \(f'(1)\).

    ??? answer "&nbsp;"

        \(
        f'(1)=-\frac{43}{4}.
        \)

#### Challenge Exercise 2: The Derivative from First Principles

Find the derivative of each function using the definition

\(
f'(x)
=
\lim_{h\to0}
\frac{f(x+h)-f(x)}{h}.
\)

You are not allowed to use differentiation rules.

1. 

    \(
    f(x)=\frac{1}{x+1}
    \)

    ??? answer "&nbsp;"

        \(
        f'(x)=-\frac{1}{(x+1)^2}.
        \)

2. 

    \(
    f(x)=\sqrt{x}
    \)

    Hint: Use the difference of two squares identity:

    \(
    (a+b)(a-b)=a^2-b^2.
    \)

    ??? answer "&nbsp;"

        \(
        f'(x)=\frac{1}{2\sqrt{x}}.
        \)

#### Challenge Exercise 3: L'Hôpital's Rule

For some limits, direct substitution gives the form \(\frac{0}{0}\) or \(\frac{\infty}{\infty}\). These are called indeterminate forms.

If both the numerator and denominator approach \(0\), or both approach infinity, the limit can often be found by differentiating the numerator and denominator separately.

L'Hôpital's rule states that

\[
\lim_{x\to a}\frac{f(x)}{g(x)}
=
\lim_{x\to a}\frac{f'(x)}{g'(x)},
\]

provided that the limit on the right-hand side exists and the original fraction has the form \(\frac{0}{0}\) or \(\frac{\infty}{\infty}\).

Use L'Hôpital's rule to evaluate the following limits:

1. 

    \(
    \lim_{x\to0}\frac{e^{2x}-1}{x}
    \)

    ??? answer "&nbsp;"

        \(
        \lim_{x\to0}\frac{e^{2x}-1}{x}=2.
        \)

2. 

    \(
    \lim_{x\to0}\frac{\sin(3x)}{x}
    \)

    ??? answer "&nbsp;"

        \(
        \lim_{x\to0}\frac{\sin(3x)}{x}=3.
        \)

3. 

    \(
    \lim_{x\to\infty}\frac{\ln(x)}{x}
    \)

    ??? answer "&nbsp;"

        \(
        \lim_{x\to\infty}\frac{\ln(x)}{x}=0.
        \)

#### Challenge Exercise 4: Optimization

A manufacturer of energy drinks wants to minimize the material costs of producing their cans.

Assume that a can can be modelled as a closed cylinder with radius \(r\) and height \(h\). The can must have a volume of \(33\) cl, corresponding to \(330\text{ cm}^3\).

The material used for the cylindrical side of the can is twice as expensive per \(\text{cm}^2\) as the material used for the top and bottom.

1. Introduce suitable variables and formulate an expression for the total material cost. You may use relative costs, where the material for the top and bottom costs 1 per \(\text{cm}^2\), while the material for the side costs 2 per \(\text{cm}^2\).

    ??? answer "&nbsp;"
        \[
        C(r,h)=4\pi rh+2\pi r^2
        \]

2. Use the volume constraint to rewrite the cost function as a function of the radius only.

    ??? answer "&nbsp;"
        \[
        C(r)=\frac{1320}{r}+2\pi r^2
        \]

3. Determine the radius that minimizes the material cost.

    ??? answer "&nbsp;"
        \[
        r=\sqrt[3]{\frac{330}{\pi}}
        \approx 4.72\text{ cm}
        \]

4. Determine the corresponding height of the can.

    ??? answer "&nbsp;"
        \[
        h\approx 4.72\text{ cm}
        \]

5. Compare your result with the case where all materials have the same cost per \(\text{cm}^2\). Explain why the optimal dimensions are different.

    ??? answer "&nbsp;"
        If all materials have the same cost, the optimal dimensions satisfy \(h=2r\).

        When the side material is twice as expensive, the optimal dimensions satisfy \(h=r\).


#### Challenge Exercise 5: Differential Equations

1. Find the function \(f(x)\) given that

    \(
    f'(x)=4x^3-6x^2+2x-1
    \)

    and

    \(
    f(1)=5.
    \)

    ??? answer "&nbsp;"

        \(
        f(x)=x^4-2x^3+x^2-x+6.
        \)

    A differential equation is an equation involving an unknown function and its derivatives. Differential equations are used, among other things, to describe population growth, cooling processes, electrical circuits and motion in physics.

    Consider the differential equation

    \(
    y'=2xy.
    \)

2. Determine whether the function \(g(x)=e^{x^2}\) is a solution to the differential equation.

    ??? answer "&nbsp;"

        Yes, \(g\) is a solution.

3. Determine whether the function \(h(x)=2e^{x^2}\) is a solution to the differential equation.

    ??? answer "&nbsp;"

        Yes, \(h\) is a solution.

4. Determine whether the function \(k(x)=e^{2x}\) is a solution to the differential equation.

    ??? answer "&nbsp;"

        No, \(k\) is not a solution.