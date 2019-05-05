# Weight and Balance

* Navigation and Radio Theory
  * Pre-flight perparation
* Flight Operations
  * Weight and Balance
  * Aircraft Performance

## Background

The distribution of weight in a glider is critical as it determines how much control authority the pilot has and
whether it is possible to recover when the aerofoils stall (e.g., in a stall or spin). As the weight distribution
moves backwards, the aircraft has an increasing tendency to fall flat and eventually even backwards. This makes
regaining control in stalls and spins increasingly difficult and eventually impossible. As the weight distribution
is moved forward, straight and level flight requires holding the stick increasingly towards its rear limit. This
increases the stall speed (we will cover why later) and leaves the pilot with very little and eventually no
backwards control authority (i.e., ability to pull the stick further back to pull up the nose of the plane if
required).

Control authority is also lost as the weight moves backwards as the stick has to be held in a further forward
position to compensate, leaving less movement available to push the nose of the plane down if required. One
situation where this is often fatal is when a tail dolly is left on the glider during take off. The pilot
frequently does not have enough forward motion in the stick to compensate, that is, establish straight and level
flight, and will crash. For this reason, making a habit of not leaving tail dollies on gliders and looking to
ensure the tail dolly has not been left on any glider you run the wing on saves lives.

The objective of this exercise is to give you and understanding of how the weight and balance calculation works so
you will not be susptible to the common mistakes that can creep in when it is instead just memorized as sequence of
operations to be performed and numbers to be compared.

As a bit of a technical aside, things have both a weight (the force gravity exerts on them) and a mass (how hard it
is to accelerate them). Generally we don't distinguish that much between these as they are just constant multiples
of each other close to the surface of the earth. That said, the imperial unit pound (lb) is actually a measure of
the latter (force), while the metric unit kilogram (kg) is the former (mass). The imperial unit for mass is slug
and the metric unit for force is newtons (N). This explains why torque wrenches are in foot-pounds and
newton-meters (not kilogram-meters).

Thinking of kilograms as a weight (force) is useful though. For this reason there is a kilograms-of-force (kgf)
unit.  It is the force a kilogram of mass experiences on the Earth's surface. This is defined to be exactly
$9.806650$N, and it is frequently approximated as a deca-newton ($10$dN). You will see both kgf and dN in European
glider manuals for this reason. Just know that a kgf (or dN) is exactly (or approximately) the weight of a kg mass
on earth (i.e., most people's understanding of a kg is not actually a kg, but rather a kgf).

## Exercise

First we introduce the idea that, from the perspective of balance, we can consider one configuration of weigths to
be equivalent to another configuration of weights.

1. Draw a balance bar with four equally spaced positions on both sides. Place a 4kg weight on the fulcrum (middle
   of the blance bar). Is the system balanced?

2. Split the 4kg weight on the fulcrum into two 2kg weights on the fulcrum and move them simultaneously outwards at
   the same rate two positions (one to the left and one to the right). Does the system remain balanced throughout
   this?

From a balancing perspective then, we can consider two separate weights to be equivalent to their combined weight
at the middle point between them.

3. With this in mind, split the weight on the left into two 1kg weights, and do the same with them. That is, move
   them outwards at the same rate two positions (one to the left and one to the right). Does the system remain
   balanced throughout this?

4. The 1kg weight that was moved to the right should now be sitting on the fulcrum again. Remove it. Does the
   system remain balanced?

From a balancing perspective then, we can consider a weight to be balanced out by another weight half its size if
it is at twice the distance. It is the combination of both weight and position that is important for determining
when a system is in balance with respect to a given fulcrum location.

5. Complete the missing weight and distance numbers for following table in order to balance the system out.  The
   left side is left and the right side is right.

   +---------+----------+--------+--------+----------+---------+
   | weight  | distance | moment | moment | distance | weight  |
   +=========+==========+========+========+==========+=========+
   |         |  $2$ m   |        |        |   $2$ m  | $2$ kgf |
   +---------+----------+--------+--------+----------+---------+
   |         |  $1$ m   |        |        |   $2$ m  | $2$ kgf |
   +---------+----------+--------+--------+----------+---------+
   | $1$ kgf |          |        |        |   $2$ m  | $2$ kgf |
   +---------+----------+--------+--------+----------+---------+

6. There is a way to combine the weight of a mass with its distance for the balancing point to get a number (the
   moment) that can be compared for the left and right sides to determine if the system is in balance. Considering
   the earier comment about twice the distance, half the weight, figure out what this is and complete the table.

The moment, or torque, is a measure of the twisting force created by the application of off-center force. It
reflects both how much force is being applied and how far it is from the point in question. This is experienced
when removing bolts: make the wrench twice as long and you only have to pull half as hard. A system is balanced
about the point where it is being twisted equally left and right. Otherwise it will rotate to the greater twist.

7. Complete the following chart by picking potential balance points and evaluating the left and right weight
   moments to figure out which are the correct ones.

   +-------------+--------------+------------+---------------+
   | left weight | right weight | separation | balance point |
   +=============+==============+============+===============+
   |    $2$ kgf  |    $1$ kgf   |   $12$ m   |               |
   +-------------+--------------+------------+---------------+
   |    $1$ kgf  |    $3$ kgf   |   $12$ m   |               |
   +-------------+--------------+------------+---------------+
   |    $2$ kgf  |    $3$ kgf   |   $12$ m   |               |
   +-------------+--------------+------------+---------------+

**If you have not completed the above exercises yet, do so before continuing to read.**

In order to find the balance point we pick a distance and calculate the moments. If they are equal, we are done. If
not, we move the point over. This increases the distance on the one side (making that moment bigger) and decreases
it on the other (making that moment smaller) in order to balance things.

What we are actually doing is solving the following equation

$$
F_l \times (d_l + \delta) = F_r \times (d_r - \delta)
$$

where $F_l$ and $F_r$ are the forces due to the weights on the left and right, $d_l$ and $d_l$ are the distances on
the left and right to our initial guess at the balance point, and $\delta$ is the amount we need to move our guess
over to the left (negative) or right (positive) in order that the left and right moments (the two sides) become
equal.

8. Solve the above equation algabraically for $\delta$.

Solving this equation should give you $\delta = (F_r \times d_r - F_l \times d_l) / (F_r + F_l)$. If adopt the
convetion that distances to the left are negative ($x_l = -d_l$ and $x_r = d_r$), this simplifies to

$$
\delta = \frac{(F_r \times x_r + F_l \times x_l)}{F_r + F_l} = \frac{\sum \text{force} \times \text{signed distance}}{\sum \text{force}}
$$

where $\sum$ means to add together. You will often see the signed distances refered to as arms. The equation says
to sum all the forces times their arms (distances, left negative and right positive) and then divide by the sum of
just the forces. This gives how far off the balance point is from the point the arms were measured from (negative
again being left and positive right).

9. Redo the prior exercise of finding the balance point using this equation.

## References

* [faa]: https://www.faa.gov/regulations_policies/handbooks_manuals/aircraft/glider_handbook/
  Glider Flying Handbook. Chapter 5 discusses weight and balance issues and calculations.

  [https://www.faa.gov/regulations_policies/handbooks_manuals/aircraft/glider_handbook/](https://www.faa.gov/regulations_policies/handbooks_manuals/aircraft/glider_handbook/)
