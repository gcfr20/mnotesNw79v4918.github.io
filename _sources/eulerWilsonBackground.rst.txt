
Background (Advanced Math Concepts)
=========================================

A congruence :math:`ax\equiv 1~(mod~n)` is equivalent to the Diophantine equation :math:`ax+ny=1`. **A solution for x exists only if gcd(a,n)=1**. Otherwise, a and n will have a common divisor different from 1, the left hand side will be divisible by this common divisor, but the right hand side will not be, leading to a contradiction.

In fact, if gcd(a,n)=1, :math:`ax\equiv 1~(mod~n)` is guaranteed to have a unique solution modulo n. If we define a binary operation - 'multiplication' - with arguments a and x as multiplication modulo n, then 1 can be defined as the identity (neutral element) for the operation, and a and x are inverses of each other.

Euler's Theorem
------------------

Consider a subset G of :math:`S=\{0,1,2,...,n-1\}` defined as the set of numbers that are relatively prime to n. Multiplication is commutative and associative, there is a multiplicative identity, and every member of the set G has a multiplicative inverse within set G. Thus, G forms a multiplicative group. The order of the group is :math:`\varphi(n)`. When any element of a multiplicative group is raised to the order of the group, the result is the mulitplicative identity. Hence, for all elements of the group G, :math:`a^{\varphi(n)}\equiv 1~(mod~n)1`. This is Euler's theorem.

=================================================   

As an example, let us consider numbers modulo 15. :math:`\varphi(15)=(3-1)(5-1)=8`.

.. list-table::
   :widths: 10, 30, 20, 20
   :header-rows: 1

   * - a
     - is gcd(a,15)=1?
     - inverse(a)
     - order of a
   * - 0
     - N
     - 
     - 
   * - 1
     - Y
     - 1
     - 1
   * - 2
     - Y
     - 8
     - 4
   * - 3
     - N
     - 
     - 
   * - 4
     - Y
     - 4
     - 2
   * - 5
     - N
     - 
     - 
   * - 6
     - N
     - 
     - 
   * - 7
     - Y
     - 13
     - 4
   * - 8
     - Y
     - 2
     - 4
   * - 9
     - N
     - 
     - 
   * - 10
     - N
     - 
     - 
   * - 11
     - Y
     - 11
     - 2
   * - 12
     - N
     - 
     - 
   * - 13
     - Y
     - 7
     - 4
   * - 14
     - Y
     - 14
     - 2
       
The order of an element :math:`a` (as opposed to order of the group) is the smallest positive integer :math:`k` such that :math:`a^k\equiv 1~(mod~n)`, that is the smallest power that gives the identity. As can be seen from the table, the order of the elements of G divide the order of the group G (a consequence of Lagrange theorem in group theory) resulting in the Euler's theorem.

=================================================   

Wilson's Theorem
------------------

Now consider the case of modulo p, where p is a prime greater than 2. Every residue other than 0 is relatively prime with p and is thus invertible. Hence, :math:`\varphi(p)=p-1` and the group G is of order :math:`p-1`.

For any modulo :math:`n`, :math:`1` and :math:`n-1` are self-inverses. For modulo prime :math:`p`, the :math:`(p-2)` residues other than :math:`1` and :math:`p-1` pair up to form pairs of mutual-inverses. Thus, multiplying these :math:`(p-2)` numbers results in :math:`(p-2)!\equiv 1~(mod~p)`.

We have not proved that the :math:`p-2` residues other than :math:`1` and :math:`p-1` cannot be self inverses. Suppose, one of those residues - :math:`q` - is a self-inverse.

.. math::

   & q^2\equiv 1~(mod~p)

   & \left(q^2-1\right)\equiv 0~(mod~p)

   & (q-1)(q+1)\equiv 0~(mod~p)

However, both :math:`q-1` and :math:`q+1` are relatively prime to :math:`p`. Thus, neither :math:`q-1`, nor :math:`q+1` is divisible by prime :math:`p`. Hence, :math:`(q-1)(q+1)` is not divisible by :math:`p` and we have a contradiction. Hence, :math:`q` cannot be a self-inverse.

=================================================   

As an example, consider modulo 11. :math:`\varphi(11)=10`.

Self-inverses:

.. math::

   & 1 \times 1 \equiv 1~(mod~11)

   & 10 \times 10 \equiv 1~(mod~11)

Inverse-pairs:
   
.. math::

   & 2 \times 6 \equiv 1~(mod~11)

   & 3 \times 4 \equiv 1~(mod~11)

   & 5 \times 9 \equiv 1~(mod~11)

   & 7 \times 8 \equiv 1~(mod~11)

Multiplying these four congruences, :math:`9!\equiv 1~(mod~11)` : Wilson's theorem 

