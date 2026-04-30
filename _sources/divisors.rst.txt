
Prime Factorization and Divisors of numbers
==============================================

Prime Factorization
----------------------

Prime factorization of any number is unique and can be obtained using either the tabular method or the tree method. It is a good idea to write the primes in increasing order.

:math:`540=2^2\times 3^3\times 5^1`

GCD and LCM
-------------

Get the prime factorization of the numbers whose GCD or LCM is desired. Pick the smallest powers for each prime present in any of the prime factorizations for the GCD. Pick the largest powers for the LCM.

.. math::

   540 &= 2^2\times 3^3\times 5^1

   210 &= 2^1\times 3^1\times 5^1\times 7^1

   1210 &= 2^1\times 5^1\times 11^2

Including all the primes that show up:

.. math::

   540 &= 2^2\times 3^3\times 5^1\times 7^0\times 11^0

   210 &= 2^1\times 3^1\times 5^1\times 7^1\times 11^0

   1210 &= 2^1\times 3^0\times 5^1\times 7^0\times 11^2

.. math::

   &\text{GCD}=2^1\times 3^0\times 5^1\times 7^0\times 11^0=10

   &\text{LCM}=2^2\times 3^3\times 5^1\times 7^1\times 11^2=457380


When only two numbers are involved, the product of the GCD and LCM is the product of the two numbers. The reason for this is that in this case the product of the smallest power and the largest power for each prime in the factorization will be the product of the powers of that prime in the two numbers.

.. math::

    & 20 = 2^2 \times 5^1

    & 250   = 2^1 \times 5^3

    & (2^1 \times 5^1) \times (2^2\times 5^3)=(2^2\times 5^1)\times (2^1\times 5^3)

    & \text{GCD}\times \text{LCM}=20 \times 250

Divisors
-------------

Consider the number 8. Its divisors are 1, 2, 4, and 8. Why are these the only divisors?

The prime factorization of :math:`8` is :math:`2^3`. Thus, the divisors are powers of :math:`2` such that the power is less than or equal to the power of :math:`2` in :math:`8`. In other words, the divisors are :math:`2^0,~2^1,~2^2,~2^3`.

Number of divisors
^^^^^^^^^^^^^^^^^^^^

By extending this logic, the divisors of :math:`72=2^3\times 3^2` will be all combinations of :math:`2^0,~2^1,~2^2,~2^3` and :math:`3^0,~3^1,~3^2`:

:math:`2^0\times 3^0,~2^0\times 3^1,~2^0\times 3^2`

:math:`2^1\times 3^0,~2^1\times 3^1,~2^1\times 3^2`

:math:`2^2\times 3^0,~2^2\times 3^1,~2^2\times 3^2`

:math:`2^3\times 3^0,~2^3\times 3^1,~2^3\times 3^2`

Thus, the total number of divisors is :math:`(3+1)\times(2+1)=12`. This is denoted by the Greek letter "tau": :math:`\tau(72)=12`.


Sum of divisors
^^^^^^^^^^^^^^^^^^

The sum of the divisors is denoted by the Greek letter "sigma".

.. math::

   \sigma(72)&= 2^0\times 3^0+2^0\times 3^1+2^0\times 3^2

   &+2^1\times 3^0+2^1\times 3^1+2^1\times 3^2

   &+2^2\times 3^0+2^2\times 3^1+2^2\times 3^2

   &+2^3\times 3^0+2^3\times 3^1+2^3\times 3^2

   &= \left(2^0+2^1+2^2+2^3\right)\left(3^0+3^1+3^2\right)

   &= 15\times 13=195


The summation in the last step can be done manually for small sums. When the numbers are large, one can note that each paranthesis in the penultimate step is the :ref:`summation of a geometric series <algebraicIdentities:Adding geometric series>`.
   
Thus,

.. math::

   \sigma(72)&= \left(2^0+2^1+2^2+2^3\right)\left(3^0+3^1+3^2\right)

   &=\left(\frac{2^4-1}{2-1}\right)\times \left(\frac{3^3-1}{3-1}\right)
   
   &= 15\times 13=195

Another example:

.. math::

   540&=2^2\times 3^3\times 5^1

   \tau(540)&=(2+1)(3+1)(1+1)=24

   \sigma(540)&=\left(\frac{2^3-1}{2-1}\right)\left(\frac{3^4-1}{3-1}\right)\left(\frac{5^2-1}{5-1}\right)=1680

Product of divisors
^^^^^^^^^^^^^^^^^^^^^

   
The product of the divisors can be obtained easily by noting that for every divisor, the number can be written as a product of the divisor and another complementary divisor. Thus, listing out the equations for all the divisors we can get the product of the divsors. See an example for the number 8 below.

.. math::

   8 &= 1 \times 8

   8 &= 2 \times 4

   8 &= 4 \times 2

   8 &= 8 \times 1

Taking the product of all the equations

.. math::

   8^4 = 8^{\tau(8)} &=(1\times 2\times 4\times 8)^2

   &= \text{Product of divisors}^2

   \text{Product of divisors} &= \sqrt{8^4}= 64

Highest power of a number that divides a factorial
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


What is the highest power of 2 that divides 12!?

Let us denote this by the Greek-letter "nu": :math:`\nu_2(12!)`

:math:`10!=1\times 2\times3\times 4\times 5\times 6\times 7\times 8\times 9\times 10\times 11\times 12`

Observe that 2, 6, and 10 contribute one power of 2 each; 4 and 12 contribute two powers of 2 each; and 8 contributes three powers of 2.

A different way of counting this is as follows: 2, 4, 6, 8, 10, and 12 contribute the first power of 2 each; 4, 8, and 12 contribute a second power of 2 each; and finally 8 contributes a third power of 2. Thus, we are counting the number of multiples of 2^1, 2^2, and 2^3 in 12!.

:math:`\frac{12}{2}=6,~\frac{12}{4}=3,~\frac{12}{8}=1.5`. Thus, we throw away the fractional part and get :math:`6+3+1=10` as the higher power of 2 that divides 12!.

The "throw away the fractional part" is handled by the greatest integer function - the largest integer that is smaller than a number is the greatest integer function. We will call it the floor function and will write it as follows:

.. math::

   \lfloor 13.24 \rfloor &= 13

We won't have to deal with negative numbers here. Nonetheless, as an example for negative numbers, :math:`\lfloor -13.24\rfloor=-14`.

Thus,

.. math::

   \nu_2(12)&=\left\lfloor \frac{12}{2^1}\right\rfloor+\left\lfloor \frac{12}{2^2}\right\rfloor+\left\lfloor \frac{12}{2^3}\right\rfloor+\left\lfloor \frac{12}{2^4}\right\rfloor+\left\lfloor \frac{12}{2^5}\right\rfloor + ...

   &=6+3+1+0+0+... = 10

In the above example, we were looking for the highest power of a prime number. What if one wants the highest power of a number that is the product of prime numbers?

What is :math:`\nu_{42}(100!)` ?

The prime factorization of 42 is :math:`2^1\times 3^1\times 7^1`. Note that we are restricting ourselves to the case where the highest power of any prime in the prime factorization is 1. Each power of 42 in 100! will come from one 2, one 3, and one 7. Moreover, powers of 2 will be more frequent than powers of 3 which, in turn, will be more frequent than powers of 7. Thus, we only need to find the highest power of 7 that divides 100!.


.. math::

   \nu_{42}(100)= \nu_{7}(100) = \left\lfloor \frac{100}{7} \right\rfloor + \left\lfloor \frac{100}{7^2} \right\rfloor = 14 + 2 = 16

Powers of 7 greater than 2 are larger than 100. Thus, the floor functions for those powers are 0.




   
