
Finding Remainders
======================================


Here we discuss the following type of questions:

What is the remainder when :math:`3^{231}` is divided by :math:`17`?

What is the last digit of :math:`29^{51}`? This is same as finding the remainder of the number when divided by 10.

What is the last two digits of :math:`29^{51}`? This is same as finding the remainder of the number when divided by 100.

The basic method to answer these questions is to use the modular arithmeic/congruences background that we have already developed. Later on, we will look at a couple of theorems that can be powerful tools.

=================================================

Finding last digits

.. math::

   2^1 &\equiv 2~(mod~10)

   2^2 &\equiv (2)(2) \equiv 4 ~(mod~10)

   2^3 &\equiv (4)(2) \equiv 8 \equiv -2 ~(mod~10)

   2^4 &\equiv (-2)(2)\equiv -4 \equiv 6 ~(mod~10)

   2^5 &\equiv (-4)(2)\equiv -8\equiv 2 \equiv 2^1 ~(mod~10)

The cycle repeats with periodicity of 4 in the powers.

Hence, the problem is more about finding the remainder when the power is divided by 4.

=================================================

For example, find the last digit of :math:`2^{1172719191911919}`

.. math::

   1172719191911919 &\equiv (11727191919119\times 100 + 19)\equiv (0 + 19)\equiv 19 \equiv 3~(mod~4)

   &\implies 2^{1172719191911919} \equiv 2^3 \equiv 8~(mod~10)

=================================================
   
Find the remainder when :math:`13^{10023}` is divided by :math:`15`.

.. math::

   13^{10023} &\equiv (-2)^{10023}~(mod~15)

   &~
   
   (-2)^4 &\equiv 16 \equiv 1~(mod~15)

   &~
   
   10023 &\equiv 23~(mod~4) \equiv 3~(mod~4)

.. math::

   \text{Hence, $(-2)^{10023}\equiv (1)(-2)^3\equiv -8~(mod~15)$}


.. math::
   
   13^{10023} \equiv -8~(mod~15) \equiv 7~(mod~15)

=================================================
   
Find the last two digits of :math:`7^{47}`

Some observations:

.. math::

   & 100 = 2^2 \times 5^2 = 4\times 25.~ \text{gcd($4$, $25$)=$1$}

   & x\equiv y~(mod~100)\implies (x-y)\equiv 0~(mod~100)\implies (x-y)\equiv 0~(mod~4)~\text{and}~(x-y)\equiv 0~(mod~25)

   &\implies x\equiv y~(mod~4)~\text{and}~x\equiv y~(mod~25)

From the section on congruences, we know how to solve such systems of congruences. If a solution exists (which we know exists for our problem), then the solution will be unique modulo :math:`\text{lcm}(4,25)=100` which is what we want for the last two digits.

.. math::

   7^{47} &\equiv (-1)^{47} \equiv -1 \equiv 3~(mod~4)

   & ~

   7^2 &\equiv 49 \equiv -1~(mod~25) \implies 7^{47} \equiv \left(7^2\right)^{23}(7)\equiv (-1)^{23}(7)\equiv -7\equiv 18 ~(mod~25)

We need to now solve the following system:

.. math::

   x &\equiv 3~(mod~4)

   x &\equiv 18~(mod~25)

The solutions to the second congruence modulo 100 are :math:`18,~43,~68,~93`. Not surprisingly, there are 4 solutions with different residues modulo 4.

The one that satisfies the first congruence is :math:`43`.

Hence, :math:`7^{47}\equiv x\equiv 43~(mod~100)`

   

   


   
   
