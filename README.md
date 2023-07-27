# DMC-Simulation-Studies-of-a-Continuous-Stirred-Tank-Reactor-with-and-without-a-Recycle

This repository contains the work we have done on developing a DMC strategy for a CSTR, a common equipment in the chemical industry. The aim is to control various parameters like reactant concentration, temperature (for temperature-varying reactions), reactant flow rates and split fractions (for recycle systems). 

Our goal is to control reactant concentration and temperature during an irreversible exothermic reaction in the reactor. The reactor is cooled by a single coolant stream, and the task is to meet concentration specifications while maintaining an optimal reactor temperature. We've referenced system parameters from Ahmed J. Abougarair's paper "Simulation Studies of Continuous Stirred Tank Reactor Using Artificial Neural Network Based Supervised Control Method", but for our project, we've employed Dynamic Matrix Control.

We've also explored a reactor system with a recycle stream back to the feed. The controller, in this case, manipulates the split fraction of the product species fed back to the reactor and the reactant flowrate to control the reactant concentration.

## Project Structure
1. Formulation of the ordinary differential equations (ODEs) that describe the CSTR’s behavior.
2. Obtaining the step response.
3. Developing a process model for the CSTR (both with and without recycle).
4. Utilizing the DMC method on this model to predict the system’s behavior over a finite time horizon.
5. Utilizing nonlinear models to accurately capture the CSTR’s behavior.

## Results

Through simulations, the DMC model was successful in meeting the concentration specifications and maintaining the optimal reactor temperature. Unfortunately, we couldn't compare results between the two cases (CSTR with and without recycle) as initially intended due to controller issues with the operation of the recycle split fraction.

Feel free to explore this repository for a detailed look at our work. Contributions and suggestions are always welcome!
