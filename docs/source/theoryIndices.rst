
Theory of Indices
======================================

In the following discussion, :math:`a` is an arbitrary real number with :math:`a\neq 0`. Thus, it has a multiplicative inverse :math:`a^{-1}` (See :ref:`axioms for real numbers <realField:Axioms for Real Numbers>` for definitions).

Integer Powers
----------------

For any positive integer :math:`n`, :math:`a^n` is defined as

.. math::

   a^n = \underbrace{a\times a \times \ldots \times a}_{\text{$n$ terms}}

and

:math:`a^{-n}` is defined as

.. math::

   a^{-n} = \underbrace{a^{-1}\times a^{-1} \times \ldots \times a^{-1}}_{\text{$n$ terms}} =  \underbrace{\frac{1}{a}\times \frac{1}{a} \times \ldots \times \frac{1}{a}}_{\text{$n$ terms}}

Here, :math:`a^{-1}` is the multiplicative inverse of :math:`a`.

Some consequences of these definitions are listed below.

.. math::

   a^2\cdot a^3&=(a\cdot a)\cdot (a\cdot a\cdot a)=a^5

   a^{-2}\cdot a^{-3}&=\left(\frac{1}{a}\cdot \frac{1}{a}\right)\cdot \left(\frac{1}{a}\cdot \frac{1}{a}\cdot \frac{1}{a}\right)=a^{-5}

   \left(a^2\right)^3&=a^2\cdot a^2\cdot a^2=a^6

   a^2\cdot a^{-3}&=(a\cdot a)\cdot \left(\frac{1}{a}\cdot \frac{1}{a}\cdot \frac{1}{a}\right)=\frac{1}{a}=a^{-1}

   \left(a^{-2}\right)^{-3}&= \left(a^{-1}\cdot a^{-1}\right)^{-3} = \left(a^{-1}\cdot a^{-1}\right)^{-1}\cdot \left(a^{-1}\cdot a^{-1}\right)^{-1}\cdot \left(a^{-1}\cdot a^{-1}\right)^{-1}

   &=\left(a^{-1}\right)^{-1}\cdot \left(a^{-1}\right)^{-1}\cdot \left(a^{-1}\right)^{-1}\cdot \left(a^{-1}\right)^{-1}\cdot \left(a^{-1}\right)^{-1}\cdot \left(a^{-1}\right)^{-1}=a\cdot a\cdot a\cdot a\cdot a\cdot a=a^6

   
Thus, in general, for any integers :math:`m` and :math:`n` (both positive and negative),

.. math::

   & a^m\cdot a^n = a^{m+n}

   & \left(a^m\right)^n = a^{m\times n}

   
By defining :math:`a^0=1`, we get consistency with the above properties.

.. math::

   & 1 = a\cdot a^{-1} = a^{1-1} = a^0

Fractional Powers
--------------------

The definitions can be extended to fractional powers maintaining consistency of the two properties above.

For positive integer :math:`n` and for any integer :math:`m` (positive, negative, or zero),

 .. math::

    a^{\frac{1}{n}} &= \sqrt[n]{a}

    a^{\frac{m}{n}} &= \left(a^{\frac{1}{n}}\right)^m

Thus,

.. math::

   \left(a^\frac{1}{n}\right)^n=\left(\sqrt[n]{a}\right)^n=a=a^1

   
 
   
