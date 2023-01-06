
Here are summaries of some of my completed projects.

## [Project 1: Zero-Age Main Sequence Star Simulator](https://github.com/cjhapich/star_simulator)

### Disclaimer
An improved version of a numerical simulation I wrote in Python as a sophomore. Most of the equations come from Carroll & Ostlie's *An Introduction to Modern Astrophysics* (2006). While I wrote the procedures myself, many of the calculations were pulled directly from Carroll & Ostlie's Fortran 95 script **STATSTAR**. Whereas **STATSTAR** integrates in radius, my code integrates in mass in an effort to more accurately calculate changes in high density regions. This code is just for fun, and I do not claim ownership of any of the methods of the simulation.

### Overview
* Takes input from the user in the form of a stellar mass, an effective temperature and luminosity, and hydrogen and metal mass ratios to compute the profile of a main sequence star at the beginning of its life (zero-age).
* Solves the differential equations of mass conservation, hydrostatic equilibrium, energy generation, and radiative or convective heat transfer with a fourth-order Runge Kutta integration. Also uses several equations of state to work backwards from the surface of the star. At the surface and center of the star, approximate functions are used to avoid dealing with derivatives that are zero or very large.
* Contains built-in options to plot profiles of the interior mass, temperature, pressure, density, interior luminosity, and nuclear energy generation as functions of radius. Also writes the results of the calculation as a .csv file.

## [Project 2: Unilluminable Room Simulation](https://github.com/cjhapich/unilluminable_room)

### Overview
* Simulation of photon motion in a 4-sided Tokarsky "unilluminable room", in which light starting at one side of the room will never make it to the other side. Used matplotlib's FuncAnimation feature to make movies of photons and rays moving through the room.

![](/images/particles.gif)

![](/images/ray_trace.gif)

* Ran simulations of 100,000 photons in an effort to measure the light distribution over the room after many reflections. Since photons are increasingly reflected backwards the farther into the room one gets, I expected to find a shadow approaching the unilluminable point. Detected a noticable shadow approaching the unilluminable side that got more pronounced as simulation step size was decreased.

![](/images/normalized_density.png)

* Plan to implement continuous collision detection to improve simulation quality. A more complete analysis is in the repository.

## [Project 3: Solar System Birthday Calculator](https://github.com/cjhapich/other_worlds_code)

### Overview
* Created a calculator that takes a date of birth and returns the date of the next birthday for 10 worlds in the solar system (the 8 planets and dwarf planets Pluto and Ceres).
* Calculator also returns the next half birthday (when someone is N + 0.5 years old), the current age, the length of the year, and the length of the birth week on each world.
* Project required analysis of the Gregorian calendar system: since the Gregorian year drifts by a non-integer number of days and corrections are only made by adding single whole days, the calculated next birthday on Earth can be off by as much as 2 days. A brief analysis is provided in the repository.

![](/images/other_worlds_example_1.png)

![](/images/other_worlds_example_2.png)
