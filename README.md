# exp_3_vi_characteristics_of_gunn_oscillator

# Experiment 3 — V–I Characteristics of Gunn Oscillator

---

## Aim

To study the I–V characteristics of a Gunn diode and the depth of modulation of a PIN diode.

## Apparatus Used

Gunn power supply, Gunn oscillator, PIN modulator, isolator, frequency meter, variable attenuator, detector mount, slotted section, VSWR meter.

## Experimental Setup

<img width="2170" height="725" alt="image" src="https://github.com/user-attachments/assets/9572ed54-7f9f-413c-b568-c08d9049d680" />

---

## Theory

The Gunn oscillator is based on the **negative differential conductivity** effect in bulk semiconductors. The Gunn diode has two conduction bands separated by an energy gap larger than thermal agitation energies. When an electron is transferred to the satellite energy band it acquires negative differential mobility, producing the negative resistance required for oscillation.

In a Gunn oscillator the diode is placed in a resonant cavity, so the oscillation frequency is set by the cavity dimensions rather than by the diode itself.

Although a Gunn oscillator can be amplitude-modulated with the bias voltage, a separate **PIN modulator** is used in this experiment: a square-wave modulating signal is applied through the modulator onto the microwave carrier.

<img width="542" height="341" alt="image" src="https://github.com/user-attachments/assets/313e43ed-dd69-4b09-9a4f-7a7616faa805" />

---

## Procedure

1. Set up the components and equipment as shown in the figure above.
2. Initially set the variable attenuator for maximum attenuation.
3. Keep the control knobs of the Gunn power supply as follows:

   | Control | Setting |
   |---|---|
   | Meter switch | OFF |
   | Gunn bias knob | Fully anti-clockwise |
   | PIN bias knob / Mod amplifier | Mid position |
   | PIN mod frequency | Mid position |

4. Keep the control knobs of the VSWR meter as follows:

   | Control | Setting |
   |---|---|
   | Meter switch | Normal |
   | Input switch | Crystal low impedance / 200 K |
   | Range dB switch | 50 dB |
   | Gain control knob | Fully clockwise |

5. Set the micrometer of the Gunn oscillator between 5–7 mm for the required frequency of operation.
6. Switch ON the Gunn power supply, the VSWR meter and the cooling fan.
7. Keep the mode switch of the Gunn power supply at square wave / internal modulation.
8. Turn the meter knob to the voltage position and note that as the Gunn bias voltage is varied the current starts decreasing — this indicates the negative resistance characteristic of the Gunn diode. Apply a voltage that puts the device in the middle of the negative resistance region.
9. Connect the detector output to the SWR meter.
10. Adjust the square-wave modulation frequency to approximately 1 kHz.
11. Change the meter range if no deflection is observed.
12. Keep the slotted-line probe at the position where maximum deflection is observed on the meter.
13. Adjust the attenuator setting and the gain control knob of the VSWR meter and tune the detector plunger so the pointer indicates VSWR = 1.
14. Move the detector probe along the slotted line and note the position where the pointer reaches the extreme left — the first minimum. To locate the minimum exactly, note the positions of equal-response points on either side; their midpoint gives the position of the minimum. Note the next minimum position the same way.
15. Repeat the above procedure for different micrometer settings.

### Depth of Modulation of the PIN Diode

1. Apply the Gunn bias voltage slowly until the panel meter of the Gunn power supply reads 8 V.
2. Tune the PIN modulator bias voltage and frequency knobs for maximum output on the oscilloscope.
3. Align the bottom of the square wave on the oscilloscope with a reference level and note the micrometer reading of the variable attenuator.
4. Now, using the variable attenuator, align the top of the square wave with the same reference level and note the micrometer reading.
5. Connect the VSWR meter to the detector mount and note the dB reading for both micrometer settings of the variable attenuator.
6. The difference between the two dB readings gives the modulation depth of the PIN modulator.

> **Note:** After tuning the Gunn source, follow the same procedure for VSWR and impedance measurement as for the depth of modulation of the PIN modulator.

## Observation

Operating Parameters:

Resonant Frequency: 9.45 GHz

Modulating Signal: 1 kHz Square Wave

Material / Type: n-GaAs Gunn Diode

Table 1: V-I Characteristics of Gunn Diode

|S.No | Gunn Bias Voltage V (V) | Diode Current I (mA) | Region of Operation |
|---|---|---|---|
1 | 0.5 | 45 | Linear / Ohmic Region
2 | 1.0 | 95 | Linear / Ohmic Region
3 | 1.5 | 148 | Linear / Ohmic Region
4 | 2.0 | 198 | Linear / Ohmic Region
5 | 2.5 | 240 | Linear / Ohmic Region
6 | 3.0 | 275 | Approaching Threshold
7 | 3.4 (Vth) | 295 (Ipeak) | Threshold Point (Peak)
8 | 3.8 | 278 | Negative Differential Resistance (NDR)
9 | 4.2 | 255 | Negative Differential Resistance (NDR)
10 | 4.8 | 225 | Negative Differential Resistance (NDR)
11 | 5.5 | 195 | Negative Differential Resistance (NDR)
12 | 6.2 | 172 | Negative Differential Resistance (NDR)
13 | 7.0 | 158 | Negative Differential Resistance (NDR)
14 | 8.0 (Vop) | 150 (Ivalley) | Stable Oscillation Point (Valley)
15 | 8.5 | 152 | Saturation / Post-Valley Region

Table 2: PIN Diode Modulation Depth

| State | Attenuator Position (mm) | SWR / Power Meter Reading (dB) | Oscilloscope Peak Voltage (Vp-p)|
|---|---|---|---|
ON State (Wave Top) | 3.25 mm | 34.2 dB | 1.85 V
OFF State (Wave Base) | 1.10 mm | 18.6 dB | 0.31 V

## Calculation

Negative Differential Resistance (Rn)
The dynamic negative resistance is computed across the active region from the threshold point (Vth, Ipeak) to the valley operating point (Vop, Ivalley):

Delta V = Vop - Vth = 8.0 V - 3.4 V = 4.6 V
Delta I = Ivalley - Ipeak = 150 mA - 295 mA = -145 mA = -0.145 A

Rn = Delta V / Delta I = 4.6 V / (-0.145 A) = -31.72 Ohms

Peak-to-Valley Current Ratio (PVCR)
PVCR = Ipeak / Ivalley = 295 mA / 150 mA = 1.97

Depth of Modulation of PIN Diode

Method A: Decibel Method (from VSWR / Power Meter)
Depth of Modulation (dB) = Reading_ON - Reading_OFF
Depth of Modulation = 34.2 dB - 18.6 dB = 15.6 dB

Method B: Percentage Modulation Method (from CRO trace)
m = [(Vmax - Vmin) / (Vmax + Vmin)] * 100%
m = [(1.85 - 0.31) / (1.85 + 0.31)] * 100%
m = (1.54 / 2.16) * 100% = 71.30%
## Precautions

* Check the connections before switching on the kit.
* Make all connections properly.
* Take the observations carefully.

## Conclusion

CONCLUSION
The current-voltage (V-I) characteristics of the Gunn diode were studied. The device demonstrated Ohmic behavior up to the threshold voltage Vth = 3.4 V with a peak current Ipeak = 295 mA.

Beyond the threshold, the diode demonstrated the transferred-electron (Gunn) effect, displaying negative differential resistance (Rn = -31.72 Ohms) with a Peak-to-Valley Current Ratio (PVCR) of 1.97.

Stable microwave oscillations were established at the recommended operating bias of Vbias = 8.0 V.

The modulation depth of the PIN diode modulator was determined to be 15.6 dB (or 71.30%), confirming effective square-wave amplitude modulation of the X-band carrier.
