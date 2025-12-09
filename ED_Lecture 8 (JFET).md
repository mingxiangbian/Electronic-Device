# Junction Field Effect Transistor
## Types of Field Effect Transistor
![[39.png|400]]
## Junction Field Effect Transistor (JFET)
JFETs are three-terminal voltage-controlled semiconductor devices that can be used to
control switches or amplifiers.![[40.png|300]]
There are two JFET types:
> n-channel and p-channel
> Similar in physical structure to a BJT
>> It is also a 3-terminal device 
>> here are two pn-junctions

However, JFET is a **Voltage Controlled Device**, as opposed to a Current Controlled Device in the case of the BJT.![[41.png|400]]
> (a) The basic structure of the junction field effect transistor (JFET) with an n-channel. The two $p^+$ regions are electrically connected and form the gate.
> (b) A simplified sketch of the cross section of a more practical _n_-channel JFET

### JFET Principles
![[42.png|400]]
> (a) The gate and source are shorted ($V_{GS} = 0$) and $V_{DS}$ is small
> (b) $V_{DS}$ has increased to a value that allows the two depletion layers to just touch. This is called pinch-off voltage, $V_{DS}$ = $V_P (= 5 V)$. Since gate to source is short, $V_{GS}$ = 0 , $V_{GD}$ = $−V_{DS}$ = −$V_P = − 5 V$. 
> (c) $V_{DS}$ is large ($V_{DS} > V_P$) so that a short length of the channel is pinched off.

![[43.png|400]]
![[44.png|200]]
> Beyond Channel Pinch-off: 
> As $V_{DS}$ increases, most of the additional voltage simply drops across $𝑙_{𝑝𝑜}$ as this region is depleted of carriers and hence highly resistive.
> Electrons in the n-channel drift toward P. When they arrive at P, they are swept across the pinched-off channel by E-field. This process is similar to minority carriers in the base of a BJT.
> Drain current, $I_D$, is actually determined by the resistance of the conducting n-channel over $L_{ch}$ from A to P. $$I_D=\frac{V_P}{R_{AP}}(V_{DS}>V_P)$$
> As $𝑉_{𝐷𝑆}$ increases, most of the additional voltage simply drops across $𝑙_{𝑝𝑜}$ as this region is depleted of carriers and hence highly resistive.

1. We first considered the behavior of the JFET with the gate and source shorted ($V_{GS}=0$). The resistance between S and D is the resistance of the conducting n-channel between A and B, $R_{AB}$.
2. When a positive voltage is applied to D with respect to S ($V_{DS}>0$), then a current flows from D to S which is called the drain current $I_D$.
3. There is a voltage drop along the channel, between A and B. The voltage in the n-channel is zero at A and $V_{DS}$ at B.
4. As the voltage along the n-channel is positive, the pn junctions between the gates and the n-channel become progressively more reverse-biased from A to B. Consequently, the depletion layers extend more into the channel and thereby decrease the thickness of the conducting channel from A to B.
5. Increasing $V_{DS}$ increases the widths of the depletion layers, which penetrate more into the channel and hence result in more channel narrowing toward the drain.
6. The resistance of the n-channel $R_{AB}$ therefore increases with $V_{DS}$. The drain current therefore does not increase linearly with $V_{DS}$.$$I_D=\frac{V_{DS}}{R_{AB}}$$
![[46.png|400]]
#### **Pinch-off condition**
$$V_{DS(sat)}=V_{P}+V_{GS}, I_D\approx I_{DS}\approx\frac{V_{DS(sat)}}{R_{AP}(V_{GS})}=\frac{V_P+V_{GS}}{R_{AP}(V_{GS})}$$
> where $V_{GS}$ is a negative voltage (reducing $V_{DS(sat)}$) and $𝑅_{𝐴𝑃}$ is the effective resistance of the n-channel from A to P.
> Beyond pinch-off when $V_{DS} > V_{DS(sat)}$, the point _P_ where the channel is just pinched still remains at potential $V_P$, thus $V_{AP}$ remains at $V_{DS(sat)}$, given by the above equation.

(1) The resistance increases with more negative gate voltage as this increases the reverse bias across the $p^+$n junction, which leads to the narrowing of the channel.
e.g. when $𝑉_{𝐺𝑆}= -4 V$, the channel thickness at A becomes narrower than in the case with $𝑉_{𝐺𝑆} = -2 V$, thereby increasing the resistance ($𝑅_{𝐴𝑃}$) of the conducting channel and therefore decreasing $𝐼_{𝐷𝑆}$.
(2) Further, there is a reduction in the drain current by virtue of $V_{DS(sat)}$ decreasing with negative $𝑉_{𝐺𝑆}$.
These two effects (i.e. from $V_{DS(sat)}$ and that from $𝑅_{𝐴𝑃}$) lead to $𝐼_{𝐷𝑆}$ almost decreasing parabolically with $−𝑉_{𝐺𝑆}$.

#### **JFET with Turn-off $V_{GS}$**
![[47.png|200]]
When the gate voltage is such that $𝑉_{𝐺𝑆} = −𝑉_𝑝 (= -5 V)$ with the source and drain shorted ($𝑉_{𝐷𝑆} =0$), then the two depletion layers touch over the entire channel length and the whole channel is closed. **The channel is said to be off.** The only drain current that flows when a $𝑉_{𝐷𝑆}$ is applied is due to the thermally generated carriers in the depletion layers. This current is very small.
When $V_{GS} = − 5 V$ the depletion layers close the whole channel from the start, at $V_{DS} = 0$. As $V_{DS}$ is increased there is a very small drain current which is the small reverse leakage current due to thermal generation of carriers in the depletion layers.

#### **JFET Transfer Characteristics**
![[48.png|400]]
#### **Beyond pinch-off**
A simple way to express the relationship between $I_{DS}$ and $V_{GS}$ is:$$I_{DS}=I_{DSS}[1-(\frac{V_{GS}}{V_{GS(off)}})]^2$$
> where, $I_{DSS}$ is the drain current when $V_{GS} = 0$ 
> $V_{GS(off)} = –V_p$; the gate-source voltage that just pinches off the channel

#### **Summary**
1. Modulating the electric field in the reverse-biased depletion layers (by changing $V_{GS}$) varies the depletion layer penetration into the channel and hence the resistance of the channel. **The transistor action hence can be thought of as being based on a field effect**. Since there is a pn junction between the gate and the channel, the name has become **JFET**. This junction in reverse bias provides the isolation between the gate and channel.
2. Secondly, the region beyond pinch-off is commonly called the current saturation region, as well as constant current region and pentode region. The term **saturation** should not be confused with similar terms used for **saturation effects in bipolar transistors**. A saturated BJT cannot be used as an amplifier, but **JFETs are invariably used as amplifiers in the saturated current region**.

### JFET Common Source Amplifier
1. The transistor action in the JFET is the control of $𝐼_{𝐷𝑆}$ by $𝑉_{𝐺𝑆}$. The input circuit is the gate-source circuit containing $𝑉_{𝐺𝑆}$ and the output circuit is the drain-source circuit in which the drain current $𝐼_{𝐷𝑆}$ flows.
2. The JFET is almost never used with the pn junction between the gate and channel forward-biased ($𝑉_{𝐺𝑆} > 0$).
3. With $𝑉_{𝐺𝑆}$ limited to negative voltages, the maximum current in the output circuit can only be $𝐼_{𝐷𝑆𝑆}$. The maximum input voltage $𝑉_{𝐺𝑆}$ should therefore give an $𝐼_{𝐷𝑆}$ less than $𝐼_{𝐷𝑆𝑆}$.
![[45.png|400]]
When the signals are small about dc values, we can use differentials to represent small signals. For example, $𝒗_{𝒈𝒔} = 𝜹𝑽_{𝑮𝑺}, 𝒊_𝒅 = 𝜹𝑰_{𝑫𝑺},𝒗_{𝒅𝒔} = 𝜹𝑽_{𝑫𝑺}$ and so on. The variation $δ𝐼_{𝐷𝑆}$ due to $δ𝑉_{𝐺𝑆}$ about the dc value may be used to define a **mutual transconductance** $𝒈_𝒎$ for the JFET.
Definition of the JFET transconductance (small signal) $$g_m=\frac{dI_{DS}}{dV_{GS}}\approx\frac{\delta I_{DS}}{\delta V_{GS}}=\frac{i_d}{v_{gs}}$$
JFET transconductance (small signal) 
$$g_m=\frac{dI_{DS}}{dV_{GS}}=-\frac{2I_{DSS}}{V_{GS(off)}}[1-(\frac{V_{GS}}{V_{GS(off)}})]=-\frac{2[I_{DSS}I_{DS}]^{1/2}}{V_{GS(off)}}$$
Small-signal voltage gain $$A_V=\frac{v_{ds}}{v_{gs}}=\frac{-R_Di_d}{v_{gs}}\to A_V=-g_mR_D$$
> The amplification can be increased by increasing $𝑹_𝑫$, but we must maintain $𝑉_{𝐷𝑆}$ at all times above $𝑉_{𝐷𝑆(𝑠𝑎𝑡)}$ (i.e. beyond pinch-off) to ensure that the drain current $𝑰_{𝑫𝑺}$ in the output circuit is only controlled by $𝑽_{𝑮𝑺}$ in the input circuit.

### BJTs and FETs Differences
![[49.png]]

