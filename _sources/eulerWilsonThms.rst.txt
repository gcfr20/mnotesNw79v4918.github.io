
Euler and Wilson's Theorems
======================================

Euler's phi function or Euler's totient function
--------------------------------------------------

Consider a positive integral power of a prime number, for example, :math:`2^4`.

**How many numbers smaller than this number are relatively prime to this number?**

x and y are relatively prime or coprime when :math:`gcd(x,y)=1`.

This number is called the Euler's phi function or Euler's totient function and is denoted by the Greek letter "phi": :math:`\varphi\left(2^4\right)`. 

Clearly, any number that divisible by 2 will have 2 as a common factor with :math:`2^4`. There are :math:`\frac{2^4}{2}=2^3` such numbers smaller than or equal to :math:`2^4`. All other numbers will be relatively prime to :math:`2^4`.

Hence, :math:`\varphi\left(2^4\right)=2^4-2^3=8`.

Thus, for any prime p and positive integer k, :math:`\varphi\left(p^k\right)=p^k-p^{k-1}`.

As a special case, for any prime p, :math:`\varphi(p)=p-1`.

The Euler's phi function is a multiplicative function (stated here without proof). **If a and b are relatively prime**, then :math:`\varphi(ab)=\varphi(a)\varphi(b)`. This can be recursively extended to more than two numbers. For example, if a, b, and c are pairwise relatively prime, then :math:`\varphi(abc)=\varphi(a)\varphi(b)\varphi(c)`.

Hence,

.. math::

   & 100 = (2^2)(5^2)

   & \varphi(100)=\varphi\left(2^2\right)\varphi\left(5^2\right) =\left(2^2-2^1\right)\left(5^2-5^1\right)=(2)(20)=40

   & ~

   & 1260 = (2^2)(3^2)(5^1)(7^1)

   & \varphi(1260)=\left(2^2-2^1\right)\left(3^2-3^1\right)(5-1)(7-1)=(2)(6)(4)(6)=288
   
We now state two theorems without proofs. A link is presented at the end of this section for some background which is advanced and can be skipped for most applications.

Euler's Theorem
----------------

**If a and n are relatively prime**, then :math:`a^{\varphi(n)}\equiv~1~(mod~n)`
.

Example: :math:`41^{\varphi(100)}\equiv 41^{40}\equiv 1~(mod~100)`

Note: :math:`2^{\varphi(100)}\equiv 2^{40} \equiv 76\neq 1~(mod~100)`. This does not contradict Euler's theorem because 2 and 100 are not relatively prime.

The special case of Euler's theorem when n is a prime is called Fermat's little theorem.

Euler's theorem is a useful tool while finding remainders.

=================================================

For example, what are the last two digits of :math:`7^{162}`?

.. math::

   & gcd(7,100) = 1,~\varphi(100)=40

   & 7^{162}\equiv \left(7^{40}\right)^4 \left(7^2\right)\equiv (1)(49)\equiv 49~(mod~100)

=================================================

What are the last two digits of :math:`7^{158}`?

Let :math:`7^{158}\equiv x~(mod~100)`.

.. math::

   & 7^{160}\equiv \left(7^{40}\right)^4\equiv 1~(mod~100)~\text{(Euler)}

   & 7^{160}\equiv \left(7^{158}\right)\left(7^2\right)\equiv 1~mod~(100)

   & 49x\equiv 1~mod~(100)

   & 100=4\times 25,~gcd(4,25)=1

   & \text{Hence, } 49x\equiv 1~(mod~4)~\text{and}~49x\equiv 1~(mod~25)

   & 49x\equiv (1)x\equiv x\equiv 1~(mod~4)

   & 49x\equiv (-1)x\equiv -x\equiv 1~(mod~25)\implies x\equiv -1\equiv 24~(mod~25)

Thus, we need solution of the system :math:`x\equiv 1~(mod~4),~x\equiv 24~(mod~25)` resulting in a unique residue modulo 100.

The second congruence short-lists the following residues modulo 100: 24, 49, 74, 99. The one that satisfies the first congruence is 49.

=================================================


Wilson's Theorem
-----------------

**If p is a prime greater than 2**, then :math:`(p-2)!\equiv 1~(mod~p)`.

For any number n, :math:`(n-1)\equiv -1~(mod~n)`. Thus, Wilson's theorem can also be written as

.. math::

   (p-1)!\equiv (p-2)!\times(p-1)\equiv (1)(-1)\equiv -1~(mod~p)

=================================================

Example: :math:`15!\equiv 1~(mod~17),~16!\equiv -1~(mod~17)`

=================================================

What is the remainder when :math:`13!` is divided by 17?

Let :math:`13!\equiv x~(mod~17)`.

.. math::

   & 15!\equiv 1~(mod~17)~\text{(Wilson)}

   & (x)(14)(15)\equiv 1~(mod~17)

   & (x)(-3)(-2)\equiv 1~(mod~17)

   & 6x\equiv 1\equiv -16~(mod~17)

   & 3x\equiv -8\equiv 9~(mod~17)

   & x\equiv 3~(mod~17)

=================================================   

.. toctree::

   eulerWilsonBackground.rst

   
