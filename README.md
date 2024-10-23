# High-fidelity-DV-entanglement-generation
These two codes are designed for heralded entangled spin generation, based on the Barret-Kok scheme and Humphrey scheme

# Generation of spin-photon entangled pair via BK protocol: 
Phys. Rev. A 71, 060310(R) (2005)

Based on the spin-photon entanglement result, we would like to develope the protocol to entangle the two spin systems with high fidelity. To start with, let's prepare two copies of spin-photon systems. In BK protocol (Phys. Rev. A 71, 060310 (2005)), there are 5 steps to achieve high fiedlity or highly entangled state and consists of 5 steps.

**Step 1:** Prepare the initial state as the equally suerposition state as: $|\psi_0\rangle=\frac{1}{\sqrt{2}}\left(|g_{\downarrow}0\rangle_A+|g_{\uparrow}0\rangle_A\right)\otimes\frac{1}{\sqrt{2}}\left(|g_{\downarrow}0\rangle_B+|g_{\uparrow}0\rangle_B\right)$.

**Step 2:** Send the optical field, whose Rabi frequency is $\Omega_s$ and is resonant to the frequency between the transition $|g_\downarrow\rangle_{s}\rightarrow|e\rangle_{s}$, to the NV system, where $s=A,B$. The interaction Hamiltonian can be written as: $\hat{H}/\hbar=\sum_{s=A,B}\Omega_s\hat{a}_s\hat{\sigma}_{+,s}$, where $\hat{\sigma}_{+,s}=|e\rangle_{ss}\langle g_{\downarrow}|$, with the excitation time-dependent Hamiltonian that uses the semi-classical approximation: $\hat{H}_{\text{exc}}\left(t\right)/\hbar=\sum_{s=A,B}P_s\left(t\right)\hat{\sigma}_{+,s}+\text{h.c.}$, where $P_s\left(t\right)$ is the Rabi frequency of the excitation pulse. For simplicity, let's assume identical Rabi frequencies, excitation pulses of system A and B as $\Omega$ and $P\left(t\right)$.

**Step 3:** Counts the clicks that occur at detector $D_1$ or $D_2$. As a reminder, $D_1$ (or $D_2$) stands for the collapsing operator of mode $\hat{a}_A+\hat{a}_B$ (or $\hat{a}_A-\hat{a}_B$).

**Step 4:** Applying both qubits (A and B) with X-gate operation individually, $\hat{X}=\left(|g_\uparrow\rangle\langle g_\downarrow|+|g_\downarrow\rangle\langle g_\uparrow|+|e\rangle\langle e|\right)_A\otimes\left(|g_\uparrow\rangle\langle g_\downarrow|+|g_\downarrow\rangle\langle g_\uparrow|+|e\rangle\langle e|\right)_B$, to flip the spins.

**Step 5:** Repeat Step 1.

In the following, we provide the codes to simulate the overall process.


# Generation of spin-photon entangled pair via Humsphrey's protocol: 
Nature volume 558, pages268–273 (2018)

Based on the spin-photon entanglement result, we would like to develope the protocol to entangle the two spin systems with high fidelity. To start with, let's prepare two copies of spin-photon systems. In Humsphrey's protocol (Nature 558, 268 (2018)), we prepare the two spin-cavity systems with initial state $$|\psi_0\rangle=\left(\sqrt{\alpha}|g_{\downarrow}0\rangle_A+\sqrt{1-\alpha}|g_{\uparrow}0\rangle_A\right)\otimes\left(\sqrt{\alpha}|g_{\downarrow}0\rangle_B+\sqrt{1-\alpha}|g_{\uparrow}0\rangle_B\right)$$, where $|g_{\downarrow}\rangle$ ($|g_{\uparrow}\rangle$) denotes the bright (dark) state and $|0\rangle$ denotes the vacuum state of the cavity mode. Afterwards, we send the resonant optical field, whose Rabi frequency is $\Omega_s$,  to the frequency between the transition $|g_\downarrow\rangle_{s}\rightarrow|e\rangle_{s}$, to the NV system, where $s=A,B$. The interaction Hamiltonian can be written as: $\hat{H}/\hbar=\sum_{s=A,B}\Omega_s\hat{a}_s\hat{\sigma}_{+,s}+\text{h.c.}$
, where $\hat{\sigma}_{+,s}=|e\rangle_{ss}\langle g_{\downarrow}|$, with the excitation time-dependent Hamiltonian that uses the semi-classical approximation: $$\hat{H}_{\text{exc}}\left(t\right)/\hbar=\sum_{s=A,B}P_s\left(t\right)\hat{\sigma}_{+,s}+\text{h.c.}$$
, where $P_s\left(t\right)$ is the Rabi frequency of the excitation pulse. For simplicity, let's assume identical Rabi frequencies, excitation pulses of system A and B as $\Omega$ and $P\left(t\right)$. Subsequently, we count the clicks that occur at detector $D_1$ or $D_2$. As a reminder, $D_1$ (or $D_2$) stands for the collapsing operator of mode $\hat{a}_A+\hat{a}_B$ (or $\hat{a}_A-\hat{a}_B$).

In the following, we provide the codes to simulate the overall process.
