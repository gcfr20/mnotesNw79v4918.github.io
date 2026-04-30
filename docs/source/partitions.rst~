
Recurrence Relations (Advanced)
======================================

The first three sections provide a flavor of recurrence relations. We pick up the thread on distributions from other sections in the fourth section on Stirling number.


Tower of Hanoi
------------------

The image below shows a classic problem where there are three pegs and a certain number of discs with distinct sizes (diameters). The discs are initially sitting on the first peg ordered by size. No disc is sitting above a disc that is smaller than its size. The objective is to move this stack of discs to the third peg following two rules: **1) Only one disc can be moved at a time, and 2) A disc can only be placed onto an empty peg, or onto a larger disc.** What is the least number of moves required to move a stack with :math:`n` discs?

.. image:: tower_of_hanoi.png
  :width: 150

If there is only **1 disc**, the move can be done in one step. We will denote this by :math:`T(1)=1`.
	  
If there are only **2 discs**, we will first move to the top small disc from peg A to peg B, then move the bottom large disc from peg A to peg C, and finally move the small disc from peg B to peg C. So we need :math:`T(2)=3` moves.

.. image:: tower_of_hanoi_soln2.png
  :width: 600
	  
Note, even though we are highlighting the peg names, the whole idea is to move the disc stack to another peg using a third peg as a temporary holding place. In the general case, it does not matter if larger discs are already present on some pegs. The top of the stack consisting of two discs can still be moved using the same algorithm irrespective of if larger discs are already present on other pegs.

Now, suppose there are **3 discs**. We can move the stack of the top two discs to peg B using the recipe for 2 discs, move the largest of the 3 discs from peg A to peg C, and then move the 2 disc stack from peg B to peg C, again using the two disc recipe.

.. image:: tower_of_hanoi_soln3.png
  :width: 600

Thus, :math:`T(3)=2\times T(2)+1`.

In fact, for any :math:`n (n>1)`, :math:`T(n+1)=2\times T(n)+1`. We can move the stack of the top :math:`n` discs to peg B, then move the largest disc from peg A to peg C, and finally move the stack of the :math"`n` discs from peg B to peg C.

Thus, we can compute T(2) from T(1), T(3) from T(2), T(4) from T(3), and so on using our formula without actually thinking about all the moves. Such formulas that are applied successively are called recurrence relations.

There are ways to solve such a formula and get explicit non-recursive answers. For example, the tower of Hanoi formula gives

:math:`T(n)=2^n-1`.

However, in this section, we do not worry about how to solve such recurrence relations. We are just highlighting the fact that such recurrence relations can be derived and successive application of such recurrence relations allows one to calculate counts for small arguments.

Fibonacci Sequence
--------------------

Another well-known recurrence relation is for the Fibonacci problem. The details of the problem can be read `at this link  <https://en.wikipedia.org/wiki/Fibonacci_sequence#Europe>`_.

This results in the following recurrence relation:

.. math::

   F(1)&= 1

   F(2)&= 1

   F(n)&=F(n-1)+F(n)~\text{(For } n>2 \text{ )}

=================================================

Combinations
------------------------------

In our discussion of basic combinatorics, we learnt that the number of ways of choosing :math:`k` objects from :math:`n` distinguishable objects is given by :math:`C(n,k)=\frac{n!}{(n-k)! k!}`.

We could make this choice in another way. Consider one of the :math:`n` objects. There are two mutually exclusive possibilities. Either this object is chosen or the object is not chosen. If the object is chosen, then we only need to choose the remaining :math:`k-1` objects from :math:`n-1` objects. If the object is not chosen, then we need to choose the :math:`k` objects from :math:`n-1` objects. Thus, applying the addition principle (corresponding to the **or** between the mutually exclusive events),

.. math::

   C(n,k) = C(n-1,k-1) + C(n-1,k)

This formula is known as Pascal's rule.

Note that :math:`C(n,0)=C(n,n)=1` for any :math:`n`. There is only one way of not choosing any object or choosing all the objects. For other :math:`k`, :math:`C(n,k)` can be obtained using the Pascal's rule recursively.
 
.. math::

   & C(0,0)=1

   & C(1,0)=1,~C(1,1)=1

   & C(2,0)=1,~C(2,1)=C(1,0)+C(1,1)=1+1=2,~C(2,2)=1

   & C(3,0)=1,~C(3,1)=C(2,0)+C(2,1)=1+2=3,~C(3,2)=C(2,1)+C(2,2)=2+1=3,~C(3,3)=1

More details about the application of Pascal's formula can be found `here <https://en.wikipedia.org/wiki/Pascal%27s_triangle>`_.

Stirling Number
-----------------

In our discussion of the :ref:`inclusion-exclusion principle <inclusionExclusion:Distinguishable Distributions>` , we had come across the following problem:

In how many ways can 12 **distinguishable** presents be given to three people such that every person gets at least one present and all the presents are given out?


We then encountered a variant of this problem in :ref:`stones and sticks principle <stonesSticks:Stones and Sticks Principle>`.

In how many ways can 12 **indistinguishable** presents be given to three people such that every person gets at least one present and all the presents are given out?

Here we study the third variant where the presents are distinguishable, but the receivers of the presents are not. Replace the persons receiving with indistinguishable robots. Alternatively, we frame an equivalent problem.

In how many ways can 12 people sit at 3 tables if the tables can be considered indistinguishable, no table is empty, and every person sits at one of the tables? In other words, only the combination of people matters; the exact table they are sitting at does not matter for counting configurations. This number is denoted by :math:`S(12,3)` and is known as the Stirling number (of the second kind).

If tables can be empty, then the problem becomes one of finding :math:`S(12,3)+S(12,2)+S(12,1)`.

This problem can be solved by using a recurrence relation.

Consider one of the 12 people. Either this person sits by himself at a table or shares the table with other people. If the person sits by himself, the other 11 people have to sit at 2 tables. Thus, the number of configurations for this case is :math:`S(11,2)`. However, if the person shares the table, then we first let the other people first sit at the 3 tables such that no table is empty (this can be done in :math:`S(11,3)` ways , and then add this person to one of the 3 tables (this can be done in 3 ways). Hence, :math:`S(12,3)=S(11,2)+3\times S(11,3)`.

For :math:`n>0,~S(n,1)=1` as there everyone has to sit at the only table available. For :math:`n<k,~S(n,k)=0` as there are more tables than people. For :math:`n>0,~S(n,n)=1` as if there are same number of people as tables, there can be only one person per table to ensure that no table is empty.

In general (for :math:`n>1,~k>1`):

.. math::

   & S(n,k) = S(n-1,k-1) + k \times S(n-1,k)

This successive recursion becomes cumbersome for large numbers. Let us calculate this for a manageable case.

.. math::

   &S(1,1) = 1

   &S(2,1) = 1

   &S(2,2)=S(1,1)+2S(1,2)=1+2\times 0 = 1

   &S(3,1) = 1

   &S(3,2)=S(2,1)+3S(2,2)=1+2\times 1=3

   &S(3,3)=S(2,2)+3S(2,3)=1+3\times 0=1

   &S(4,1) = 1

   &S(4,2)=S(3,1)+2S(3,2)=1+2\times 3=7

   &S(4,3)=S(3,2)+3S(3,3)=3+3\times 1=6

   &S(4,4)=S(3,3)+4S(3,4)=1+4\times 0=1
   
   

