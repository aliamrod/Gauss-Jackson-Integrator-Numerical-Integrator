# Gauss-Jackson-Integrator-Numerical-Integrator


The Gauss integration scheme is a very efficient method to perform numerical integration over intervals. If the function to be integrated is a polynomial of an appropriate degree, then the Gauss integration scheme products exact results. 
The Gauss integration scheme has been implemented in almost every finite element analysis software due to its simplicity and computational efficiency.

The GJI is a sophisticated numerical method for solving second-order ODEs. It is utilized by NASA in the simulation of orbital dynamics, outperforming the Verlet method by several orders of magnitude. In general, it can be used to solve initial value problems (IVPs) of the following kinds: 

    - solve a single second-order ODE
    - solve a system of second-order ODEs
    - solve a system of first-order ODEs, by first writing as a system of second order ODE

  In the following repository, I have provided implementations of GJ Numerical Integrators in Python.  



## Additional Information

The GJ ODE solver attempts to numerically solve a second-order ordinary differential equation in the form: y''(t) = f(t, y(t))

for the value of the function _y_ at times _t_ = 0, _h_, _2h_, _3h_, ...

Here, _f_ is an arbitrary function, and _y_ could be a scalar or vector function. For instance _y(t)_ might be the 3D position of a satellite at time _t_, and _f(t,y(t))_ might return the acceleration of the satellite at the given time at the given position. Or _f_ could be a simpler function, and our ODE could be something like: y''(t) = -y(t) + tsin(2t)

which has the closed-form solution

y(t) = c1cos(t) + c2sin(t) - (4/3)cos(2t) - (1/3)tsin(t), where c1 and c2 are constants (these may be determined by i.e. initial conditions). 


