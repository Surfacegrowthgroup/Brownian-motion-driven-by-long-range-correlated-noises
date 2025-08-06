# Simulation codes and data for "Brownian motion driven by long-range correlated noises: From normal diffusion to superdiffusion"

## Contents

There are two MATLAB code files and text files containing data and figures. Simulations and results of the paper can be obtained using these codes. Some information is as follows.

### Running environment

All of the codes work with MATLAB R2022b. We integrate simulation and data processing into one program and output results. Therefore, it only needs to be run once to obtain the data results.

The two code files correspond to one-dimensional Brownian motion driven by long-range correlated noise and two-dimensional Brownian motion driven by long-range correlated noise, respectively. Each file includes: (i) Particle trajectories of the system; (ii) Displacement distribution; (iii) Numerical simulations of the mean squared displacement.

### 1D and 2D Brownian motion driven by long-range correlated noise

The files "BM_1D and BM_2D" are used to simulate the Brownian motion driven by long-range correlated noise in different dimensions. It has seven parameters and two functions. The meanings of the parameters are shown in the table below.

| Parameter        | Meaning                                |
| ---------------- | -------------------------------------- |
| eta               | the long-range correlated noise  |
| eta_x , eta_y         | the transverse and longitudinal long-range correlated noise  |
| max_lag      | the total time steps                   |
| msd                | the mean squared displacement            |
| theta               | the noise correlation exponent    |
| alpha               | the diffusion exponent           |
| rep           | the repeat times                       |


The subdirectories "BM_1D" and "BM_2D" each contain three computational modules: "MSD.m", "Displacement_Distribution.m", and "Trajectory_Morphology.m". These modules employ the function "fast_fractional_gaussian_noise_matlab" to mathematically transform Gaussian white noise into long-range temporally correlated noise (denoted as "eta"). Subsequently, they perform numerical simulations for: Particle trajectories, Displacement distributions, and the Mean Squared Displacement (MSD) of one-dimensional (1D) or two-dimensional (2D) Brownian motion systems. The MSD calculations utilize the function "compute_msd". After data processing, display the graphical results of the simulations.