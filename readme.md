Symbolic Derivation of the Muscle Moment Arm Matrix (OpenSim v4.0)
---

[https://github.com/opensim-org/opensim-core](OpenSim) is a framework for
modeling and simulation of musculoskeletal systems. The muscle moment arm is an
important variable for evaluating the effectiveness of a muscle to actuate a
particular joint. Calculating the muscle moment arm requires knowledge of the
muscle path and wrapping surfaces. OpenSim is restricted to evaluate the muscle
moment arm at an arbitrary configuration (e.g., $R(q) \in \mathcal{R}^{n x m}, q
\in \mathcal{R}^{n}$ with $n$ degrees of freedom and $m$ muscles), lacking the
information for calculating higher order derivatives (e.g., $\partial R(q) /
\partial q$). This project evaluates the moment arm at different configurations
and approximates its terms using multivariate polynomial fitting, thus a
symbolic expression is derived.


![Moment arm of vas_int_r at knee joint](vas_int_r_knee_angle_r.png)

![Moment arm of tib_ant_r at knee joint](tib_ant_r_ankle_angle_r.png)

Dependencies
---

- OpenSim: python wrappings [Tested Version](https://github.com/mitkof6/opensim-core/tree/stable_2)
- sympy: `pip install sympy`
- numpy: `pip install numpy`
- matplotlib: `pip install matplotlib`
- multipolyfit: `pip install multipolyfit` for multivariate polynomial fitting


<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img
alt="Creative Commons License" style="border-width:0"
src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is
licensed under a <a rel="license"
href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution
4.0 International License</a>.