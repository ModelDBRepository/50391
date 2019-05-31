This NEURON implementation qualitatively reproduces the phenomena described in 
Chow, C.C. and White, J.A.
Spontaneous action potentials due to channel fluctuations.
Biophysical Journal 71:3013-3021, 1996

An exact reproduction of their figures is not possible for the following reasons:
--differences in the pseudorandom number generators
--differences in numerical integration methods
--differences in the algorithms used to govern channel state 
  transitions

If this doesn't auto-launch, use NEURON to load init.hoc

When first loaded, this code automatically emulates part of Figure 2.
With minor modifications, it can be used to generate data for Figures 1, 3, and 4; 
however, note that this will require prolonged, repeated simulations.

On a 2 GHz PC, ~1600 seconds are needed to simulate 30 seconds of activity 
in a 100 um2 patch of membrane.

NOTE: this relies on the ChannelBuilder's ability to simulate stochastic
channels, which requires NEURON v. 5.7 or later.

