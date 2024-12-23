
Partial Fractions
===========================================

This section is mainly to present some background for the topic of telescopic summation. We limit ourselves to easy cases.

Consider a fraction of polynomials as follows:

.. math::

   \frac{8x+21}{(2x+3)(x-3)}

The denominator contains two degree 1 polynomials with no common factors and the numerator is of degree 1. This discussion is applicable even if the the numerator is a constant i.e. of degree 0. For example,

.. math::

   \frac{2}{(2x+3)(x-3)}

Both these expressions can be put in the form

.. math::

   \frac{A}{2x+3} + \frac{B}{x-3}

where :math:`A` and :math:`B` are constants (no terms in :math:`x`). If the numerator is to have any :math:`x` term, then the quotient of the division will be non-zero. However, the quotient in the case of the original fraction is zero as the degree of the numerator is lower than the degree of the denominator.

The constants :math:`A` and :math:`B` can be found as follows:

.. math::

      &\frac{8x+21}{(2x+3)(x-3)}  =  \frac{A}{2x+3} + \frac{B}{x-3} = \frac{A(x-3)+B(2x+3)}{(2x+3)(x-3)} 

      &~
      
      &8x+21 = A(x-3) + B(2x+3)~(I)

      &\text{Plug in the root of $2x+3=0$ i.e. $x=-\frac{3}{2}$ in $(I)$}

      &8\left(-\frac{3}{2}\right)+21 = A\left(-\frac{3}{2}-3\right) + B (0)\implies A=-2

      &\text{Plug in the root of $x-3=0$ i.e. $x=3$ in $(I)$}

      &8\cdot 3 + 21 = A(0)) + B (2\cdot 3 +3)\implies B=5

      &\text{Thus,}

      &\frac{8x+21}{(2x+3)(x-3)}  =  \frac{-2}{2x+3} + \frac{5}{x-3}

      




   
 

   

   

   
