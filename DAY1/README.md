# Circuit design and SPICE Simulation 

## Topics Covered :

### 1. Introduction to Circuit design and SPICE Simulation

### 2. NMOS Different regions of Operations

### 3. Introduction to SPICE

## 1. Introduction to Circuit design and SPICE Simulation :

* We have All logic gates available, like AND , OR, NOT, etc.. So All this logic cells are formed with NMOS and PMOS connection in very perticular fashion.

* By connecting all logic cells in perticular manner, and if it gives required functionality of gates or circuit then it is called as circuit design.

* Circuit design is like how we connect NMOS and PMOS in perticular fashion so that we can get the required functionality of the circuit.

* After this design that perticular circuit is fad in with waveforms to find the output characteristics, that is about SPICE simulation.



<img width="750" height="421" alt="image" src="https://github.com/user-attachments/assets/c173f704-b0c7-4f74-a08d-421fb7ae59de" />

* So in above image the NMOS and PMOS are connected in perficular fashion and it works as CMOS inverter so that is one of the example of the circuit design.

## SPICE Simulation :

* In SPICE, as we fad in waveforms of NMOS and PMOS to the circuit , then we get waveform in SPICE simulation. The waveforms decides the delay of each cell. and based on delay values, we can tune the W/L ratio of each transistor in the circuit.

* SPICE involves characterizing the NOMS and PMOS transistor in detail, means any CMOS logic in detail.


## Introduction to NMOS different operating regions :

* An NMOS (N-channel Metal-Oxide-Semiconductor) transistor is a type of MOSFET used in digital and analog circuits. It consists of a p-type substrate with two n-type regions (source and drain), separated by a channel, and a gate insulated by an oxide layer. The transistor operates based on the voltages applied to the gate (Vgs), drain (Vds), and source (typically grounded).

* The behavior of the NMOS transistor is divided into three main regions of operation: Cut-off, Linear (Resistive Operation), and Saturation.

* NMOS :
  
   * 4 Terminal device
 
   * Consists of p-substrate
 
   * Isolation Region ( SiO2 )
 
   * n+ diffusion region
 
   * Gate Oxide
 
   * Poly Silicon or Metal gate
 
   * G - Gate
 
   * S - Source
 
   * D - Drain
 
   * B - Body


### 1. Cut-off Region

Conditions: Vgs < Vth (regardless of Vds).

* Brief Explanation: In this region, the gate voltage is below the threshold, so no inversion layer (conducting channel) forms between source and drain. The transistor acts like an open switch, with negligible current flow. Any small leakage current is typically ignored in ideal models.

* Drain current:
     * Id = 0

* This is the simplest region, as the transistor is effectively off.


### 2. Linear Region 

* Conditions: Vgs ≥ Vth and Vds < (Vgs - Vth).
  
* Brief Explanation: Here, a conducting n-channel forms due to Vgs exceeding Vth. The channel is uniform along its length because Vds is small, so the transistor behaves like a voltage-controlled resistor. Current flows proportionally to Vds, and the channel is not pinched off.

* Drain Current :
    * Id = kn.(Vgs - Vt).Vds , (linear and function of Vds)
 

### 3. Saturation Region  

* Conditions: Vgs ≥ Vth and Vds ≥ (Vgs - Vth).

* Brief Explanation: As Vds increases beyond (Vgs - Vth), the channel pinches off near the drain end, limiting further current increase with Vds. The current becomes relatively constant (saturates) and depends mainly on Vgs. This region is ideal for amplification in analog circuits or as a current source, and it's the "on" state in digital logic.

* Drain Current :
     * Id = [kn'/2.(W/L).(Vgs - Vt)^2.(1 + λ.Vds)]
 

  
 

  













