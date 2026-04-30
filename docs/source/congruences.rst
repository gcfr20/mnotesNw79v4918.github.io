
Congruences
======================================


Some principles can be used to solve congruences are listed below

1) Common factors principle I

   Common factors between the left side, residue, and the modulus can be
   removed

.. math::

   &(ak)x\equiv (bk)~(mod~ck)\implies ax\equiv b~(mod~c)

   &\text{Example}

   &12x\equiv 6~(mod~21)\implies 4x\equiv 2~(mod~7)

2) Common factors principle II

   After all the common factors have been removed using principle I,
   we know that the left side and the modulus are relatively prime. Similarly, the residue and the modulus are relatively prime. In that case, any common factors between just the left side and the residue can be removed

.. math::

   &(ak)x\equiv (bk)~(mod~c),~gcd(ak,c)=1,~gcd(bk,c)=1\implies ax\equiv b~(mod~c)

   &\text{Example}

   &4x\equiv 2~(mod~7)\implies 2x\equiv 1~(mod~7)

3) Modulo simplification if possible

   :math:`a` and :math:`b` in :math:`ax\equiv b~(mod~c)` can be replaced with any equivalent numbers modulo :math:`c`

.. math::

   &\text{Example}

   &-6x\equiv 8~(mod~7)

   &\text{Replace $-6$ by $1$ and $8$ by $1$}

   &-6\equiv 1~(mod~7),~8\equiv 1~(mod~7)

   &-6x\equiv 8~(mod~7)\implies x\equiv 1~(mod~7)

After applying 3., 2. can be checked again.

Finally, the congruence can be solved by trying out remainders

.. math::

   &\text{Example}

   &2x\equiv -1~(mod~7)

   &\text{results in}

   &x\equiv 3~(mod~7)

Diophantine Equations
-----------------------

A Diophantine equation can be converted into an equivalent congruence and solved

We will assume that a solution exists. We won't check for the existence of a solution.

:math:`ax+by=c` can be written as :math:`ax\equiv c~(mod~b)` or :math:`by\equiv c~(mod~a)`

:math:`ax-by=c` can be written as :math:`ax\equiv c~(mod~b)` or :math:`by\equiv -c~(mod~a)`

.. math::

   &7x+17y=251

   &17y\equiv 251~(mod~7)

   &\text{Applying 3.}

   &3y\equiv 6~(mod~7)

   &\text{Applying 2.}

   &y\equiv 2~(mod~7)

This means :math:`y=7t+2` where :math:`t` is any integer. Plugging this back in the original equation

.. math::

   &7x+17y=251

   &7x+17(7t+2)=251

   &7(x+17t)=251-17(2)=217

   &x+17t=31

   &x=31-17t

   
Solving simultaneous congruences
---------------------------------

First, solve each congruence using the technique specified above

.. math::

   &12x~\equiv 6~(mod~10)\implies 6x~\equiv 3~(mod~5)\implies x~\equiv 3~(mod~5)

   &4x~\equiv 2~(mod~3)\implies 2x~\equiv 1~(mod~3)\implies x~\equiv 2~(mod~3)

   &2x~\equiv 1~(mod~21)\implies x~\equiv 11~(mod~21)

   &~

   &\text{Simplified system}

   &x~\equiv 3~(mod~5)

   &x~\equiv 2~(mod~3)

   &x~\equiv 11~(mod~21)

The solution is going to be modulo the lcm of the three modulos. :math:`lcm(5,3,21)=105`

Start with largest modulo and list out the residues modulo the lcm

.. math::

   x~\equiv 11~(mod~21)\implies x~\equiv \text{ (one of }11,~32,~53,~74,~95)~(mod~105)

Now consider the second larget modulo and retain only the compatible residues modulo the lcm


.. math::

   x~\equiv 3~(mod~5)\implies x~\equiv 53~(mod~105)

This result satisfies the thrid congruence in the system :math:`x\equiv 2~(mod~3)` and nothing further needs to be done. If, instead, we had more than one residues in this step, the final congruence would have been used to select the compatible single residue from the set.


   
