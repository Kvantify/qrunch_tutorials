<img width="2331" height="732" alt="Kvantify Qrunch logo" src="https://github.com/user-attachments/assets/8596aa28-bad1-4986-a237-f2ecbca7a8cf" />

# Tutorials
This is the official repository for the [Kvantify Qrunch](https://www.kvantify.com/products/qrunch) tutorials. Each folder contains one tutorial and the files required by the tutorial. For each tutorial, a working conda environment with `qrunch` installed is required. To find out how to install `qrunch`, please see the [installation instructions](https://qrunch.docs.kvantify.net/docs/getting_started.html). It is recommended to use the tutorials in combination with an IDE with code-completion, please see [our setup instructions for various IDEs](https://qrunch.docs.kvantify.net/docs/getting_started.html#setting-up-your-ide-for-a-better-experience-optional).

_**Get [Qrunch Basic](https://www.kvantify.com/products/qrunch/pricing/register) for free!**_

### Butyronitrile dissociation
<img width="355" height="200" alt="Butyronitrile" src="https://github.com/user-attachments/assets/89a734ce-65f3-48d6-9447-c723c1cc7bef" />

In this tutorial, the dissociation reaction (C≡N) of the nitrile group in the butyronitrile molecule is calculated. This system is relevant for applications in lithium-ion batteries and solar cell technologies. Various variational algorithms are used to approximate the ground state energies along the dissociation path, and these are compared to numerical solutions of the relevant subspace.

### Carbon capture with COF-999
<img width="250" height="142" alt="COF-999 " src="https://github.com/user-attachments/assets/79c91c48-d57e-4b36-aa90-0fd0e6c6e163" />

COF-999, a promising material for direct air carbon capture, shows enhanced CO<sub>2</sub> uptake in humid conditions. In this tutorial, we will calculate approximate transition state energies of CO<sub>2</sub> binding to the COF-999 organic framework with and without a water molecule. We will show that the transition state energy is lowered in the presence of water, irrespective of the reaction mechanism.

### Covalent ligand binding
<img width="450" height="252" alt="Covalent ligand" src="https://github.com/user-attachments/assets/4c5c4263-9fad-4ff2-8219-0641de0d2c11" />

In this tutorial, we will learn how to run calculations to describe the bound and unbound states of a ligand binding covalently to a target protein. For this purpose, we will use the BEAST-VQE algorithm, an approximate quantum algorithm intended to scale large active-space sizes. BEAST-VQE uses a hard-core boson approximation and thus maps two spatial orbitals to one qubit. Some of the benefits are the particularly simple forms of excitation operators and Hamiltonian groups.

### Dehalogenase reaction
<img width="250" height="245" alt="image" src="https://github.com/user-attachments/assets/55ff8e06-8338-40cd-8507-8a6a7d06f883" />

Here, we run a variational algorithm to estimate the energy of a molecule undergoing a bimolecular nucleophilic substitution S<sub>N</sub>2 reaction catalyzed by the Dehalogenase enzyme. These enzymes offer an extremely efficient and environmentally friendly method for degrading haloalkane compounds, which are potent pollutants, and could thus be useful for bioremediation tasks.

### Ionization potentials

In this tutorial, we use a variational algorithm to estimate the ionization energy of an ammonia molecule at equilibrium geometry. Doing so, we perform two single-point energy calculations, one for the neutral and one for the ionized states, where for the latter an open-shell doublet spin state is required. This gives us the ionization energy as the energy difference between the cation and neutral species.

## qBraid Instructions

After launching on qBraid, run the following in the terminal to register the license:

```bash
ENV_PATH=$(qbraid envs list | grep "Kvantify Qrunch" | awk '{print $NF}')
"$ENV_PATH/pyenv/bin/qrunch.license" add "$ENV_PATH/license.txt" --overwrite
```
