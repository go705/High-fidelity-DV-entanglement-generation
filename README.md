# High-fidelity-DV-entanglement-generation
These two codes are designed for heralded entangled spin generation, based on the Barret-Kok scheme and Humphrey scheme.

## Generation of spin-photon entangled pair via BK protocol
Reference: Phys. Rev. A 71, 060310(R) (2005)

Based on the spin-photon entanglement result, we aim to develop the protocol to entangle two spin systems with high fidelity. Initially, let's prepare two copies of spin-photon systems. The BK protocol involves 5 steps to achieve a high fidelity or highly entangled state:

**Step 1:** Prepare the initial state as the equal superposition state: 
$|\psi_0\rangle = \frac{1}{\sqrt{2}}\left(|g_{\downarrow}0\rangle_A + |g_{\uparrow}0\rangle_A\right) \otimes \frac{1}{\sqrt{2}}\left(|g_{\downarrow}0\rangle_B + |g_{\uparrow}0\rangle_B\right).$

**Step 2:** Send the optical field, whose Rabi frequency is $\Omega_s$ and is resonant to the frequency between the transition $|g_\downarrow\rangle_{s} \rightarrow |e\rangle_{s}$, to the NV system, where $s=A,B$. The interaction Hamiltonian can be written as:
$\hat{H}/\hbar = \sum_{s=A,B}\Omega_s\hat{a}_s\hat{\sigma}_{+,s} + \text{h.c.},$
where $\hat{\sigma}_{+,s} = |e\rangle_{ss}\langle g_{\downarrow}|$, with the excitation time-dependent Hamiltonian that uses the semi-classical approximation:
$\hat{H}_{\text{exc}}(t)/\hbar = \sum_{s=A,B}P_s(t)\hat{\sigma}_{+,s} + \text{h.c.},$
where $P_s(t)$ is the Rabi frequency of the excitation pulse. For simplicity, let's assume identical Rabi frequencies, excitation pulses of system A and B as $\Omega$ and $P(t)$.

**Step 3:** Count the clicks that occur at detector $D_1$ or $D_2$. As a reminder, $D_1$ (or $D_2$) stands for the collapsing operator of mode $\hat{a}_A + \hat{a}_B$ (or $\hat{a}_A - \hat{a}_B$).

**Step 4:** Apply the X-gate operation to both qubits (A and B) individually:
$\hat{X} = \left(|g_\uparrow\rangle\langle g_\downarrow| + |g_\downarrow\rangle\langle g_\uparrow| + |e\rangle\langle e|\right)_A \otimes \left(|g_\uparrow\rangle\langle g_\downarrow| + |g_\downarrow\rangle\langle g_\uparrow| + |e\rangle\langle e|\right)_B,$
to flip the spins.

**Step 5:** Repeat Step 1.

## Generation of spin-photon entangled pair via Humphrey's protocol
Reference: Nature volume 558, pages 268–273 (2018)

Based on the spin-photon entanglement result, we aim to develop the protocol to entangle two spin systems with high fidelity. Initially, let's prepare two copies of spin-photon systems in Humphrey's protocol:
$$|\psi_0\rangle = \left(\sqrt{\alpha}|g_{\downarrow}0\rangle_A + \sqrt{1-\alpha}|g_{\uparrow}0\rangle_A\right) \otimes \left(\sqrt{\alpha}|g_{\downarrow}0\rangle_B + \sqrt{1-\alpha}|g_{\uparrow}0\rangle_B\right),$$
where $|g_{\downarrow}\rangle$ ($|g_{\uparrow}\rangle$) denotes the bright (dark) state and $|0\rangle$ denotes the vacuum state of the cavity mode. Subsequently, we send the resonant optical field, whose Rabi frequency is $\Omega_s$, to the frequency between the transition $|g_\downarrow\rangle_{s} \rightarrow |e\rangle_{s}$, to the NV system, where $s=A,B$. The interaction Hamiltonian can be written as:
$\hat{H}/\hbar = \sum_{s=A,B}\Omega_s\hat{a}_s\hat{\sigma}_{+,s} + \text{h.c.},$
with the excitation time-dependent Hamiltonian that uses the semi-classical approximation:
$\hat{H}_{\text{exc}}(t)/\hbar = \sum_{s=A,B}P_s(t)\hat{\sigma}_{+,s} + \text{h.c.},$
where $P_s(t)$ is the Rabi frequency of the excitation pulse. Subsequently, we count the clicks that occur at detector $D_1$ or $D_2$.

These protocols provide the groundwork for simulations aimed at generating high-fidelity entangled states in quantum information science.
