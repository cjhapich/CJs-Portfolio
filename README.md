# CJ Portfolio
Here is a summary of my completed projects

## [Project 1: Unilluminable Room Simulation](https://github.com/cjhapich/unilluminable_room)

### Overview
* Simulation of photon motion in a 4-sided Tokarsky "unilluminable room", in which light starting at one side of the room will never make it to the other side. Used matplotlib's FuncAnimation feature to make movies of photons and rays moving through the room.

![](/images/ray_trace.mp4)


![](/images/particles.gif)

* Ran simulations of 100,000 photons in an effort to measure the shadow created by the many reflections. Detected a noticable shadow approaching the unilluminable side that got more pronounced as simulation step size was decreased.

![](/images/normalized_density.png)

* Plan to implement continuous collision detection to improve simulation quality.

## [Project 2: Solar System Birthday Calculator](https://github.com/cjhapich/other_worlds_code)

### Overview
* Created a calculator that takes a date of birth and returns the date of the next birthday for 10 worlds in the solar system (the 8 planets and dwarf planets Pluto and Ceres)
* Calculator also returns the next half birthday (when someone is N + 0.5 years old), the current age, the length of the year, and the length of the birth week on each world
* Project required analysis of the Gregorian calendar system: since the Gregorian year drifts by a non-integer number of days and corrections are only made by adding single whole days, the calculated next birthday on Earth can be off by as much as 2 days. A brief analysis is provided in the repository

![](/images/other_worlds_example_1.png)


![](/images/other_worlds_example_2.png)
