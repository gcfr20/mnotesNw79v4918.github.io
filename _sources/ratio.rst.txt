
Ratio and proportion, Variation
======================================

Ratio and proportion
------------------------

Terms such as :math:`3x`, :math:`4xy`, :math:`7x^2y^3` are polynomials with just one term. They are called monomials. The degree of a monomial is the sum of the powers on the variables. Thus, the degree of :math:`3x`, :math:`4xy`, and :math:`7x^2y^3` are 1, 2, and 5, respectively. A constant without any variables such as :math:`3` has degree 0 (it is as if the powers of variables are all 0).

Look at the following example problems:


.. math::

   &\frac{3p-5q}{7p+11q}=8,~\frac{p}{q}=?

   &\text{Let }\frac{p}{q}=k,~p=qk

   &\frac{3p-5q}{7p+11q}=8\implies \frac{3qk-5q}{7qk+11q}=8\implies \frac{3k-5}{7k+11}=8

   &\implies 3k-5=8(7k+11) \implies k=-\frac{93}{53}

======================================
   
.. math::

   &\frac{a}{b}=\frac{7}{2}, \frac{a-2b}{3a+7b}=?

   &k=\frac{7}{2},~a=kb

   &\frac{a-2b}{3a+7b}=\frac{kb-2b}{3kb+7b}=\frac{k-2}{3k+7}=\frac{3}{35}

======================================

In both cases, a fraction is given and one needs to find another fraction. The key feature of these fractions is that **the numerator and the denominator are made from two variable monomials of the same degree. In this case, the above approach of setting one variable to be proportional to the other variable works because only the constant of proportionality - k - remains in the fractions**.

Here is another example:

.. math::

   & \frac{2x+3y}{3x+y}=\frac{11}{6},~\frac{5x-4y}{6x-7y}=?

   & y=kx

   & \frac{2x+3y}{3x+y}=\frac{2+3k}{3+k}=\frac{11}{6} \implies 12+18k=33+11k \implies k=3

   & \frac{5x-4y}{6x-7y}=\frac{5-4k}{6-7k}=\frac{5-12}{6-21}=\frac{7}{15}

======================================

Another example where constant of proportionality is useful:

.. math::

   & x+y+z=81,~\frac{x}{2}=\frac{y}{3}=\frac{z}{4},~y=?

   & \frac{x}{2}=\frac{y}{3}=\frac{z}{4}=k\implies x=2k,~y=3k,~z=4k

   & x+y+z=81\implies k(2+3+4)=81\implies k=9\implies y=3k=27

   
Variation
--------------

In problem involving variations, the known information is genrally how one variable varies when another variable is varied.

For example, if a car is driven at a constant speed for twice as long, the distance covered will be twice as long (if everything else such as speed is held constant). This is written as

.. math::

   d\propto t~\text{or}~t\propto d

Distance is directly proportional to time or time is direction proportional to distance. We know that doubling the time will double the distance. However, we don't know how much distance is covered in a given time. We can find this out by converting the propotionality to an equality. For this, we need the speed. Distance covered (d) is speed (r) times the time (t). 

.. math::

   d = rt
   
This constant value that needs to be multiplied to convert proportionality to an equality is called the constant of proportionality. In this example, it is the speed. In a general example, it will have some other meaning. Nonetheless, it is needed to convert proportionality to an equality.


======================================

Here is another example:

The gravitational force (F) that the sun exerts on a planet is directly proportional to the mass of the planet (m) and inversely proportional to the square of the distance of the planet from the sun (d). In other words, if distance is held constant, doubling the mass doubles the force. If mass is held constant, doubling the distance drops the force to a quarter of the original force.

.. math::

   & F\propto m~\text{or}~m\propto F

   & F\propto \frac{1}{d^2}~\text{or}~\sqrt{F}\propto \frac{1}{d}~\text{or}~d\propto\frac{1}{\sqrt{F}}

Note how the second proportionality was reversed. To convert this into a single formula, a constant of proportionality - k - needs to be introduced.

.. math::

   F = k\times\frac{m}{d^2}

======================================

Some more examples:

   
25 horses (H) eat 5 bags of corn (B) in 12 days (D), how many bags of corn will 10 horses eat in 18 days?

.. math::

  &D \propto B~\text{(Number of days is directly proportional to number of bags)}

  &D \propto \frac{1}{H}~\text{(Number of days is inversely proportional to number of horses)}

  &D=\frac{kB}{H}~\text{(Combine proportionalities into a single equation by introducing constant of proportionality - $k$)}

  &12=\frac{5k}{25}~\text{(I)}

  &18=\frac{kB}{10}~\text{(II)}

  &\text{Dividing (II) by (I),}

  &\frac{18}{12}=\frac{B}{10}\times\frac{25}{5}\implies B=3


======================================

A bundle of hay (H) can be finished by 3 cows (c) in 8 days (d). In how many days will 2 cows finish the bundle if all the cows eat at the same rate?

.. math::

   &d\propto \frac{1}{c}~\text{(More the cows, fewer the days)}

   &d=\frac{k}{c}

   &8=\frac{k}{3}~\text{(I)}

   &d=\frac{k}{2}~\text{(II)}

   &\frac{d}{8}=\frac{k}{2}\times\frac{3}{k}

   &d=\frac{8\times 3}{2}=12
   
What happens if we introduce more variables or write the proportionality in a different way? Let us try.

.. math::

   &H\propto c~\text{(More the cows, more the hay needed if number of days constant})

   &H\propto d~\text{(More the days, more the hay needed if number of cows constant})

   &H=kcd

   &H=k\times 3\times 8~\text{(I)}

   &H=k\times 2\times d~\text{(II), note: amount of hay is the same as in (I)}

   &\text{Dividing (II) by (I)}

   &1=\frac{2d}{3\times 8}\implies d=\frac{3\times 8}{2}=12~\text{(Same answer as before)}
   
======================================

Another example:

A person's BMI (body mass index) varies directly as their weight and inversely as the square of their height. Given a person who weighs 180 pounds and is 60 inches tall has a BMI of 35.2, what is the BMI for  someone who is 150 pounds and 68 inches tall?

.. math::

   &BMI \propto w

   &BMI \propto \frac{1}{h^2}

   &BMI=\frac{kw}{h^2}

   &35.2=\frac{180k}{60^2}~\text{(I)}

   &BMI=\frac{150k}{68^2}~\text{(II)}

   &\text{Dividing (II) by (I)},

   &\frac{BMI}{35.2}=\frac{150}{68^2}\times\frac{60^2}{180}\implies BMI\approx 22.83
   
