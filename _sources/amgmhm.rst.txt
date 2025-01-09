
Arithmetic, geometric, and harmonic means
===========================================

Terms are in harmonic progression if their reciprocals are in arithmetic progression.

Almost all harmonic progression problems are solved by studying the arithmetic progression of the reciprocals.

Arithmetic mean
---------------------

.. math::

   \frac{a+b}{2},~\frac{a+b+c}{3},~\frac{a+b+c+d}{4}

Geometric mean
-----------------

.. math::

   (ab)^{\frac{1}{2}},~&(abc)^{\frac{1}{3}},~(abcd)^{\frac{1}{4}}

   &\text{or}

   \sqrt{ab},~&\sqrt[3]{abc},~\sqrt[4]{abcd}

  
Harmonic mean
-----------------

.. math::

   \frac{2}{\frac{1}{a}+\frac{1}{b}},~\frac{3}{\frac{1}{a}+\frac{1}{b}+\frac{1}{c}},~\frac{4}{\frac{1}{a}+\frac{1}{b}+\frac{1}{c}+\frac{1}{d}}

Inequalities
--------------

For positive real numbers only:

.. math::

   AM \geq GM \geq HM

The equalities happen when the numbers whose mean is being taken are equal

AM-HM looks like

.. math::

   &\left(a+b\right)\left(\frac{1}{a}+\frac{1}{b}\right)\geq 4

   &\left(a+b+c\right)\left(\frac{1}{a}+\frac{1}{b}+\frac{1}{c}\right)\geq 9

AM-GM looks like

.. math::

   &\frac{a+b}{2}\geq \sqrt{ab}

   &\frac{a+b+c}{3}\geq \sqrt[3]{abc}

Applications
--------------

For any two variables :math:`a` and :math:`b`, when the sum is fixed, the product is maximum when :math:`a=b`; when the product is fixed, the sum is minimum when :math:`a=b`.


**For a rectangle, the area is the product of the sides and the perimeter scales as the sum of the sides. Thus, for a fixed perimeter, the area is maximum when the rectangle is a square. For a fixed ares, the perimeter is minimum when the rectangle is a square.**

===========================================

Given that :math:`x` and :math:`y` are positive real numbers related by :math:`3x+2y=36`, what is the largest value that :math:`xy` and :math:`xy^2` can take?

Part 1:

.. math::

  & \frac{3x+2y}{2}\geq \sqrt{(3x)(2y)} \implies \frac{36}{2}\geq \sqrt{6}\cdot \sqrt{xy}

  & \left(\frac{18^2}{6}\right) = 54 \geq xy

  & \text{This largest value of $54$ occurs when $3x=2y=\frac{36}{2}=18$ i.e. when $x=6$ and $y=9$}

Part 2:

.. math::

  & \frac{3x+y+y}{3}\geq \sqrt[3]{(3x)(y)(y)} \implies \frac{36}{3}\geq \sqrt[3]{3}\cdot \sqrt[3]{xy^2}

  & \left(\frac{12^3}{3}\right) = 576 \geq xy^2

  & \text{This largest value of $576$ occurs when $3x=y=\frac{36}{3}=12$ i.e. when $x=4$ and $y=12$}

===========================================


We will now look at a couple of **advanced examples**. If we are dealing with power of two variables :math:`p` and :math:`q`, the AM-GM inequality has the general form

.. math::

   x\cdot p^mq^n + y\cdot p^uq^v + z\cdot p^fq^g \geq C\left(p^mq^n\times p^uq^v\times p^fq^g\right)^k

We have lumped all numerical constants into :math:`C` and written the appropriate power as :math:`k`. Our applications will not require :math:`C` and :math:`k`. Hence, the lumping. :math:`x`, :math:`y`, and :math:`z` are numbers (not variables).

For example,

.. math::

   3x^2y^3 + 5xy^2 + 7xy \geq C\left(x^2y^3\times xy^2\times xy\right)^k = C\left(x^4y^6\right)^k = C\left(x^2y^3\right)^{2k} = C\left(x^2y^3\right)^s~\text{(where $s=2k$)}

===========================================   

Advanced example:

What should be the ratio of the height to the radius of a cylinder if for a fixed total surface area of the cylinder (including the two caps), the volume of the cylinder is maximum?

.. math::

   & h:~\text{Height}
   
   & t:~\text{The ratio of height to radius}
   
   & r:~\text{Radius}

   & S:~\text{Total surface area}

   & V:~\text{Volume}

   & S = 2\pi r h + 2\pi r^2 = 2\pi r^2 (t + 1)

   & V = \pi r^2 h = \pi r^3 t

We want to vary the two knobs :math:`r` and :math:`t` such that :math:`S` is fixed and :math:`V` is maximized. We can ignore the constant multiples in the analysis.

For fixed :math:`r^2(t+1)`, maximize :math:`r^3 t`.

An attempt at applying AM-GM inequality (ignoring any numerical constant multipliers on the left) gives us

.. math::

   & r^2t + r^2 \geq C\left(r^4 t\right)^k

The problem is that we need some power of :math:`r^3 t` on the right hand side. The above inequality does not give us that. We have :math:`r^4 t`.

Next, let us try splitting either the first term or the second term (on the left hand side) needs to be split into a certain number of equal parts.

First try to split the second term into two equal parts (still ignoring numerical constants on the left. Hence no 1/2 multipliers).

.. math::

   & r^2t + r^2 + r^2 \geq C\left(r^6t\right)^k~\text{($C$ and $k$ are different from the previous usage)}

We have :math:`r^6 t`, not :math:`r^3 t`.

Next, split the first term into equal parts.

.. math::

    & r^2t + r^2t + r^2 \geq C\left(r^6t^2\right)^k = C\left(r^3t\right)^s

This time, we have our :math:`r^3 t` combination.

Now, we write the left hand side including the numerical multipliers in the correct ratio.

.. math::

   & 2\pi r^2 (t + 1)\sim \frac{r^2t}{2} + \frac{r^2t}{2} + r^2

   & \frac{r^2t}{2} + \frac{r^2t}{2} + r^2 \geq C\left(r^3t\right)^s

The right hand side will take the maximum value when the terms on the left hand side are equal.  The first two terms are already equal by choice. Thus, the first and the third terms need to be equal.

.. math::

   & \frac{r^2 t}{2} = r^2 \implies t=2

Therefore, the volume is maximized when the height is twice the radius.
   
===========================================

Advanced example:

The volume of a right triangular prism is V. The base of the prism is an equilateral triangle. What must be the side of the equilateral triangle for the total surface area of the prism to be the least?

.. math::

   & s:~\text{Side of the equilateral triangle}

   & h:~\text{Height of the prism}

   & A_b:~\text{Area of the base}

   & A:~\text{Total surface area of the prism}

   & A_b = \frac{\sqrt{3}}{4} s^2

   & V = A_b h = \frac{\sqrt{3}}{4} s^2h

   & A = 2A_b + 3sh = \frac{\sqrt{3}}{2} s^2 + 3sh

In this problem :math:`V` is fixed. Thus, :math:`s^2 h` is fixed. The objective is to minimize :math:`A`. The terms in the sum here (ignoring numerical constants) are :math:`s^2` and :math:`sh`.

Following the same strategy as the preceding problem, we are looking for the :math:`s^2 h` combination on the right hand side.

The split that will give us this combination is

.. math::

   s^2 + sh + sh \geq C\left(s^4h^2\right)^k = C\left(s^2h\right)^w

Including the numerical multipliers in the correct ratio,

.. math::

   \frac{\sqrt{3}}{2} s^2 + \frac{3}{2} sh + \frac{3}{2} sh \geq C\left(s^2 h\right)^w

For fixed right hand side, the left hand side will take minimum value when the left hand side terms are equal. The second and third terms are already equal. We need to equate the first two terms.

.. math::

   \frac{\sqrt{3}}{2} s^2 = \frac{3}{2} sh \implies h=\frac{s}{\sqrt{3}} \implies V = \frac{\sqrt{3}}{4}s^2h = \frac{s^3}{4} \implies s = \sqrt[3]{4V}

   
   
  



   
