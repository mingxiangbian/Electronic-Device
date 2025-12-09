## p-n Junction (1)
### Semiconductor Manufacturing

Wafer Manufacturing $\to$ Oxidation $\to$ Photolithgraphy $\to$ Etching $\to$ Deposition and Ion Implantation $\to$ Metal Wiring $\to$ Electrical Die Sorting $\to$ Packaging

**Wafer Manufacturing**: The main material used for making semiconductors integrated circuits 
![[1.png|200]]

**Oxidation**: The process of making the foundation of the transistor by forming a silicon oxide film on the wafer surface. Protects and blocks leakage current between circuits
![[2.png|200]]
**Photolithgraphy**: The process of drawing circuits on the wafer
**Etching**: The process of making patterns that form the semiconductor. Removing parts other than necessary circuit patterns
![[3.png|200]]
**Etching**: The process of making patterns that form the semiconductor. Removing parts other than necessary circuit patterns![[4.png|200]]
**Deposition**: making a thin film that protects, distinguishes and connects each circuit.
**Ion Implantation**: giving electrical properties to semiconductors
![[5.png|200]]
**Metal wiring**: The process of linking the metallic wires so that electrical signals are delivered well![[6.png|200]]
**EDS**: Checking whether each chip has reached the desirable quality level through electrical property testing
**Packaging**: The process of making paths for chips to exchange signals externally, and forming them to be safely protected from various external environments


### How p-n junction is formed?
#### Fabrication of p-n junction
	Oxidation – protects the wafer’s surface
	Photolithography – drawing circuits onto a wafer
	Etching – completion of circuit pattern
	Deposition & Ion Implantation – electrical properties
	Metal Wiring – electrical highways
	EDS – Testing for the desired quality

![[7.png|400]]
#### p-n junction
	Diffusion Driven by Concentration Gradient
	Holes diffuse from the p-type region to the n-type region, followed by recombination.
	Electrons diffuse from the n-type region to the p-type region, followed by recombination.

![[8.png]]
#### Depletion Region ⇔ Space Charge Region
![[9.png]]
	Depletion region contains essentially no mobile charge carriers.
	Ionized dopants remain fixed and contribute to a net charge, which is why the depletion region is also called the space charge region.
	Built-in voltage across the p-n junction.
### Characteristics of the p-n junction
#### Steady State: Diffusion = Drift
![[10.png]]
	Built-in voltage → drift current (in the opposite direction as diffusion)
	Steady state: where diffusion current equals drift current
$$V_{bi}=\frac{kT}{q}\ln{(\frac{N_DN_A}{n_i^2})}$$
	k: Boltzmann constant ($1.38\times10^{-23}J/K$), 
	T: is the absolute temperature in Kelvin (300K)
		$\frac{kT}{q}=259mV$, at $T=300K$
	q: charge of an electron ($1.6\times10^{-19}C$), 
	$N_A(acceptor)$ and $N_D(donar)$ typical values $10^{16}$ to $10^{19} cm^{-3}$ 
	$n_i$: The intrinsic carrier concentration 

Typical built-in voltages: 

| Semiconductor | Vbi (V) |
| :-----------: | :-----: |
|      Si       |  0.78   |
|      Ge       |  0.37   |
|     GaAs      |  1.21   |
#### Depletion Width
	The depletion region's width affects the diode's behaviour, including its capacitance and the 
	characteristics of the electric field.
At steady state, For a silicon: $\epsilon_r=11.7$, $\epsilon_0=8.854\times10^{-14}F/m$
$$W=\sqrt{\frac{2\epsilon_0\epsilon_rV_{bi}}{q}(\frac{1}{N_A}+\frac{1}{N_D})}$$
The total charge on the n-side must be equal to that on the p-side side for overall charge neutrality, so
$$N_AW_p=N_DW_n$$

### Forward-bias ans reverse-bias
• Biasing a p-n junction means applying an external voltage to control electrical behaviour.
• Biasing changes the depletion region width.
• A diode is a device that allows current to flow in one direction while blocking it in the opposite direction.
	Zero bias: No external voltage is applied
	Forward bias:  Positive Terminal ↔ p-type and Negative Terminal ↔ n-type (depletion region gets smaller)
	Reverse bias: Positive Terminal ↔ n-type and Negative Terminal ↔ p-type (depletion region gets bigger)
During biasing, almost all of that voltage falls across the depletion region.
$$W=\sqrt{\frac{2\epsilon_0\epsilon_r(V_{bi}-V)}{q}(\frac{1}{N_A}+\frac{1}{N_D})}$$
![[11.png|100]]
Compared to the original equation, the applied voltage either increase or decrease the built-in voltage, resulting in a junction voltage $V_{bi}-V$
	Small depletion width →  increases diffusion current due to lower electric field/potential barrier
	Large depletion width →  decreases diffusion current due to higher electric field/potential barrier

### Diode Equation
![[12.png|200]]
Ideal diode (Shockley) Equation
$$I=I_0(e^{qV/kT}-1))$$
	In forward bias (positive voltage), the current increases exponentially with voltage.
	In reverse bias (negative voltage), the current approaches the small reverse saturation current $I_S$ .

## p-n Junction (2)
![[13.png|400]]
### Junction Capacitance
![[14.png|200]]
Separation of charge leads to Capacitance
$$C=A\sqrt{\frac{qε}{2(V_{bi}-V)}(\frac{N_DN_A}{N_D+N_A})}$$
For $p^+$-n junction $N_a>>N_d$
$$C=A\sqrt{\frac{qε}{2(V_{bi}-V)}N_D}$$
Therefore, Measuring C will help extracting $N_D$ —— a common approach in manufacturing industry
### Carrier action
#### Carrier Transport
![[15.png|400]]
Primary types of carrier action occur inside a semiconductor:
	Drift: Charged particle motion under the influence of an electric field.
	Diffusion: Particle motion due to concentration gradient or temperature gradient.
#### Drift
![[16.png]]
E is applied across a semiconductor, the resulting force on the carriers tends to accelerate the +q charged holes in the direction of E and the -q charged electrons in the direction opposite to E.
This force superimposes on the random motion of electrons. Can be viewed as particles moving at a constant average drift velocity $v_d$.
![[17.png|400]]
	When electrons and holes are placed in E, they accelerate because of the force applied.
	Force on a charged particle: F = qE
	The force causes acceleration: a = F/m
	The electric field causes the particle to accelerate depending on its charge and effective mass
**Drift velocity** ($v_d$) is the velocity of charge carriers in a material when an electric field is applied. At low electric field:
$$v_d=\mu E$$
$\mu$ is the mobility of the charge carriers (how easily they move through the material).
	The mobility of electrons ($\mu_e$) and holes ($\mu_e$) differ and depend on temperature, doping concentrations and other factors.
**Drift current density** (J) refers to the flow of electric current per unit area due to the movement of charge carriers in a semiconductor under the influence of an electric field.
$$J_n=qnv_d=qn\mu_nE, J_p=qpv_d=qp\mu_pE$$
Each type of carrier contributes to the total current density based on its concentration and drift velocity.
$$J_{drift}=J_{n,drift}+J_{p,drift}$$

#### Conductivity and Resistivity
**Conductivity ($\sigma$)** : It is defined as the coefficient of proportionality between the current density (𝐽) and the electric field (𝐸) applied across the material. The overall conductivity of a semiconductor:
$$\sigma=q(n\mu_{n}+p\mu_p)$$
**Resistivity** measures how strongly a material opposes the flow of electric current. It is influenced by the number of charge carriers and how easily they move through the material.
$$\rho=\frac{1}{\sigma}=\frac{1}{q(n\mu_{n}+p\mu_p)}$$

#### Diffusion
**Diffusion** is caused by the random thermal motion of charge carriers, leading to a net flow from areas of higher concentration to lower concentration.
The diffusion current density (J) of electrons and holes is described by Fick’s Law:
$$J_{n,diffusion}=-qD_n\frac{dn}{dx}\ J_{p,diffusion}=qD_p\frac{dp}{dx}$$
	The diffusion current depends on the concentration gradient ($\frac{dn}{dx},\frac{dp}{dx}$) and the diffusion coefficients ($D_n, D_p$) for the respective charge carriers.
**Diffusion coefficient** describes how readily charge carriers move from regions of high concentration to low concentration due to a concentration gradient.
D is related to its mobility via the Einstein relation:
$$D_n=\mu_n\frac{kT}{q},\ D_p=\mu_p\frac{kT}{q}$$
	Both depend on carrier mobility and temperature, and higher mobility leads to higher diffusion rates.
	This relation connects the thermal motion of charge carriers (diffusion) to their response to an electric field (drift).

### Net Carrier Current in Semiconductors
The total or net carrier current in a semiconductor arises as the combined result of drift and diffusion currents.
$$J=J_n+J_p=J_{n,drift}+J_{n,diffusion}+J_{p,drift}+J_{p,diffusion}$$


## p-n Junction (3)
### Band Diagram of p-n junction
![[18.png|200]]
	As a result of diffusion, the energy bands bend at the junction.
	The conduction band (CB) and valence band (VB) of the n-type and p-type materials are at different energy levels.
	The bending creates a potential barrier that must be overcome for the current to flow.
	The position of the Fermi level must be the same in both p and n sides.

#### Forward Bias
![[19.png|200]]
	The applied voltage is in opposition to the built-in potential and lowers the potential barrier at the junction.
	 The depletion region narrows as more charge carriers (holes from the p-side and electrons from the n-side) are injected into the junction.
	 Electrons from the n-type region are pushed toward the p-type region, and vice-versa, increasing recombination and current flow.
#### Reverse Bias
![[20.png|200]]
	The applied voltage increases the potential barrier at the junction.
	The depletion region expands as more charge carriers are pulled away from the junction, increasing the width of the region devoid of carriers.
	Only minority carriers (electrons in p-type and holes in n-type) contribute to the small reverse saturation current, which remains nearly constant regardless of the applied reverse voltage.

#### Thermal Generation
![[21.png|200]]
	Thermal generation is the process where **electron-hole pairs** are generated due to thermal energy. 
	At any T above absolute zero, some electrons in the VB gain enough energy to jump into the CB. This process generates electron-hole pairs.
	In the band diagram, thermal generation can be visualized as electrons being excited from the VB to the CB, leaving behind holes in the VB.

### Reverse Breakdown
![[22.png|400]]
The p-n junction breaks down either by the Avalanche or Zener breakdown mechanisms, which lead to large reverse currents.
#### Avalanche Breakdown
![[23.png|200]]
	The field in the Depletion region can become so large (an increase of reverse bias) that an electron drifting in this region can gain sufficient KE to impact a Si atom and ionize it, or rupture a Si–Si bond.
	The phenomenon by which a drifting electron gains sufficient energy from the field to ionize a host crystal atom by bombardment is termed **impact ionization**.
	The EHPs generated by impact ionization themselves can now be accelerated by the field and will themselves give rise to further EHPs by ionizing collisions and so on, leading to an avalanche effect.
![[24.png|200]]

#### Zener Breakdown
![[25.png|200]]
	Heavily doped p-n junctions, (narrow W, large E)
	For a sufficient reverse bias (typically <10 V), Ec on the n-side may be lowered to be below Ev on the p-side.
	This means that electrons at the top of the VB in the p-side are now at the same energy level as the empty states in the CB in the n-side.
	As the separation between the VB and CB narrows, electrons easily tunnel from the VB in the p-side to the CB in the n-side, which leads to a current (**Zener effect**).
	The Zener effect is crucial for the operation of Zener diodes, enabling precise voltage regulation in various electronic applications.

### Calculating Junction Current in p-n Junctions
Useful tools:
1. 质量作用定律: 在特定温度下(热平衡时, $n_0$是电子总浓度, $p_0$是空穴总浓度)$$n_0 p_0=n_i^2 $$(normally, $n_i=1.5\times 10^{10}$)
2. 电中性条件: 在均匀掺杂的P型半导体中，正电荷总量等于负电荷总量. 正电荷主要来自电离的受主和空穴. 在$N_a >> n_i$下, 为简化，认为多子（空穴）浓度($p_0$)近似等于受主掺杂浓度: $$p_0\approx N_a$$
3. 因此，P型区（下标用p）的热平衡电子浓度（即少子浓度）为$$n_{p0}=\frac{n_i^2}{N_a}$$
4. 反向偏置: 当V为负且$|V|>>V_T$时, exp(qV/kT) $\to$ 0, 电流基本等于反向饱和电流
5. Due to $$qV_{bi}={kT}\ln{\frac{N_DN_A}{n_i^2}}=E_{ip}-E_{F}+(E_F-E_{in})$$![[26.png|200]]
 6. Therefore, $$E_{ip}-E_F=kT\ln\frac{N_a}{n_i}, E_F-E_{in}=kT\ln\frac{N_d}{n_i}$$
