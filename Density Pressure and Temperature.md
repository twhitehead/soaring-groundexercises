# Density, Pressure, and Temperature

* Meterology
  * The Earth's Atmosphere
  * Atmospheric Pressure
  * Meteorological Aspecfs of Altimetry
  * Temperature
  * Stability and Instability
  * Wind
  * Air Masses
  * Fronts
  * Frontal Weather
* Theory of Flight
  * Principles of Flight
  * Forces Acting on a Glider
  * Aerofoils
  * Design the Wings
  * Load Factor
* Flight Instruments
  * Pitot Static System
  * Airspeed Indicator
  * Variometer
  * Altimeter
* Flight Operations
  * General
  * Aircraft Performance
  * Wake Turbulance
  * Aircraft Critical Surface Contamination

## Background

Key properties of a gas (air in our case) are its density, pressure, and temperature. A basic understanding of these
quantities goes a long way to understanding how both aircrafts and weather work.  Working through the following
exercises will hopefully give a mental picture of what these properties are and some associated intuition.  While
it does not contain much references to aviation, it sets the stage for further discussion, as witnessed by the
large number of exam sections it is relevant to above.

## Exercise

1. Air is composed of many many tiny air molecules whizzing around in random directions colliding with themselves
   and the walls of any container they many be contained in. Draw a box with several air molecules whizzing around in
   it.  Indicate a little bit of their path with a dotted line. Include ones bouncing off the walls of the
   container and even each other.

One of the characteristics of your picture is the number of air molecules in the container. This will depend on the
size of the box you drew. All else being equal, if you drew a bigger box, you will have put more air molecules in
it than if you drew a smaller box. For this reasons, it generally isn't useful to talk about the number of air
molecules independent of the size of the box. We don't want to be talking about size all the time though, so we
divide the number of air molecules (as measured by their combined $kg$ of mass) by the volume of the box (as
measured by its $m^3$ volume).  This gives density ($kg/m^3$). It tells us how crowded it is in the box without
worrying about overall numbers and size.

2. Consider the box you drew. What would happen to the density if we changed things so there was

   * double the number of air molecules, same amount of space
   * half the number of air molecules, same amount of space
   * same number of air molecules, double the amount of space
   * same number of air molecules, half the amount of space
   * double the number of air molecules, double the amount of space
   * half the amount of air molecules, double the amount of space

When an air molecule bounces off the walls of the container, it exerts a force on it (i.e., in the collision the
air molecule pushes the wall outwards and the wall pushes the air molecule back inwards). As before, the total
average number air-molecule-wall collisions that occur each second (and hence the total average outwards force
being exerted on the walls each second) is tied to how much surface area we are talking about. Again, we don't want
to always be talking about size, so we divide the average force exerted on the wall (as measured in $N$ [Newtons]
of force) by the area of the wall (as measured in $m^2$ of surface area). This gives us pressure ($N/m^2$). It
tells us how how concentrated the force of the bombardment of the walls is without having to worry about the
overall numbers and size.

3. Consider the average number of times an air molecule bounces off the walls of the container you drew in a
   second. What would happen to this collision rate, and the associated pressure, if

   * it was twice as crowded in the container (twice the density)
   * it was half as crowded in the container (half the density)

4. Now consider how fast the air molecules are moving on average. The total force being exerted on the wall is a
   combination of how many collisions there are and how hard those collisions are. Consider doubling the average
   speed of the air molecules, would

   * the rate of collisions: double, remain the same, or half
   * the forces associated with the collisions: double, remain the same, or half
   * the pressure on the wall: quadruple, double, remain the same, half, or quarter

The fact that the speed of the air molecules counts both for the number of collisions and the force of those
collisions means we actually care about the square of the velocity (velocity times velocity). Note this as velocity
counting twice, that is, being squared, happens a lot (gust factors, lift, stoping distances, etc.). The square of
the velocity gives kinetic energy (energy due to motion). This gives temperature (as measured in $K$ [Kelvin],
which is just Celcius shifted so $-273.15^{\circ}C$, the point at which the random motion ceases, becomes $0K$). As
you may have experienced, when the air molecules are moving very fast (high termperature), their collisions with
your skin can even cause damage.

The entirety of the above can be summarized in a mathematically equation that says for a large range of conditions
(certainly those encountered in gliding) pressure is proportional to density times temperature in a gas (i.e., $P =
R \rho T$ for some constant $R$). This is know as the ideal gas law. You may have encountered it in school. You
don't need to recite it, but it is good to have a picture in your head of how density ($\rho$), pressure ($P$), and
temperature ($T$) fit together. We will relate it to aviation and weather going forward.

5. Technically the air molecules can be moving as whole in a certain direction (e.g., when the wind is blowing). It
   is only the random motion on top of this coordinated motion that counts towards temperature. This relates back
   to the different types of pressure. Static pressure is purely the pressure due to the random motion. Impact
   pressure (a.k.a., stagnation and pitot pressure) is the pressure due to both coordinated and random
   motion. Dynamic pressure is the pressure due to just coordinated motion. Using this knowledge, explain why

   * the pitot tube is on the front of the aircraft
   * the static ports are on the side of the aircraft

6. For each of density, pressure, and temperature, summarize (in a sentance or two) what quantity they are
   measuring of the air.

## References

* [faa]: https://www.faa.gov/regulations_policies/handbooks_manuals/aircraft/glider_handbook/
  Glider Flying Handbook. Chapter 9 introduces air properties and Chapter 4 covers instruments.

  [https://www.faa.gov/regulations_policies/handbooks_manuals/aircraft/glider_handbook/](https://www.faa.gov/regulations_policies/handbooks_manuals/aircraft/glider_handbook/)
