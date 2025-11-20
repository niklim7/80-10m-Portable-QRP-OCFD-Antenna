# 80-10m 7 band Portable QRP OCFD Antenna

Project Status: Completed and on the air.

## 1. Summary (Product Vision)

This project documents the design, build, and field-testing of a high-performance, portable 80-10 meter Off-Center Fed Dipole (OCFD) antenna. The design is based on the proven theory by Rick DJ0IP but modified for a QRP/portable use case with a focus on lighter wire and a custom-built, ruggedized 4:1 hybrid balun.

The goal is to create a robust, multi-band antenna system for 2-day contests or multi-day camping operations where performance and reliability are more critical than minimum weight.

## 2. Design & Requirements

Base Design: DJ0IP OCFD (80m model).

Modifications: Lighter antenna wire (vs. QRO models) and a custom-built balun.

Mast: Designed for a 14m fiberglass mast (Spiderbeam HD).

Power: Primarily for QRP (5-10w), but the balun was over-engineered to handle 50w QRO (e.g., from an RGO ONE) for future-proofing.

Key Requirement: Must be able to withstand the rigors of frequent portable assembly and disassembly.

## 3. Technical Challenge & Solution: The Hybrid Balun

The most critical component of this design is the 4:1 hybrid balun, which includes a common-mode choke.

Initial Plan: Use a lightweight FT82-61 core for the 4:1 unun and a single FT82-43 for the choke.

Expert Consultation & Risk Analysis: In an email exchange with the original designer (Rick DJ0IP), he expressed concern that a single FT82-43 core might not efficiently suppress common-mode currents on the 80m band, even at QRP levels. This was a critical risk, as common-mode current would skew resonance and SWR.

Engineered Solution: To mitigate this risk, I "beefed up" the choke by using a stack of four FT82-43 cores. I also strengthened the 4:1 unun with a 2-stack of FT82-61 cores (wound with 0.6mm enameled wire) to safely handle 50w.

Final Assembly: The coaxial used to wind the choke was a thin but rugged Teflon-coated RG178 (1.9mm OD).

## 4. Trade-off Decisions (Prioritizing Robustness)

A key decision was to prioritize ruggedness over minimum weight.

Enclosure: While the original designer recommends a simple plate, I used an ABS enclosure to protect the balun's small enameled wire and coax from mechanical stress during transport and setup.

Potting: The balun was potted in Electrolube ER 2188 electronics epoxy.

Pro: Makes the unit "mechanically immortal" and aids in heat dissipation at 50w.

Con: This critical decision increased the balun's final weight to 251g, a significant but acceptable trade-off for reliability.

## 5. Field Test 1: Deployment & Initial Data (Paneion Mtn, ~650m ASL)

Setup: This was the first field setup of the 14m Spiderbeam mast. Preparation (clamps, guy ropes) was time-intensive in 35°C heat, but future setups will be much faster.

Deployment Challenge: The plan to use a pulley for tuning was not ideal, as the mast-top bent and tangled the wires. The antenna was secured at its full height (13m feedpoint) for testing.

Initial SWR Data (Untrimmed):

80m: 1.25 @ 3.350 MHz

40m: ~1.5

12m: ~1.2

Other bands (30, 20, 15, 10m): ~2.0-4.0 (requires trimming)

Signal Validation (No QSOs): As light was fading, I packed up before making contacts. However, I confirmed the antenna was working:

The radio's tuner could tune all 7 bands.

My signal was picked up by the Reverse Beacon Network (RBN) on 40m-15m.

I could clearly hear my own signal on 80m via a nearby remote SDR.

## 6. Photos

![Image](https://github.com/user-attachments/assets/9b9bff4e-4a1b-455a-96b8-ac01e6e5637d)

![Image](https://github.com/user-attachments/assets/b41b6212-18f9-49b9-ba5a-d6a35880524e)

<img width="1080" height="2424" alt="Image" src="https://github.com/user-attachments/assets/2d6c10e7-4dfa-4547-881d-72432272106f" />

![Image](https://github.com/user-attachments/assets/5ad54fb3-dbca-4b4c-9623-9e728789cea4)

![Image](https://github.com/user-attachments/assets/1c248ecf-eaee-4bc3-80d4-bcc033f22075)

![Image](https://github.com/user-attachments/assets/d6c557d0-7af5-47d4-a68b-b00f76f98ccd)

![Image](https://github.com/user-attachments/assets/03bce4e1-7309-428d-9346-53e3c4be640a)

![Image](https://github.com/user-attachments/assets/0b18955b-5213-4b46-b6c4-93bc39016cdf)

![Image](https://github.com/user-attachments/assets/2ac42c7b-ee78-48bc-94ac-214f277d83a5)

![Image](https://github.com/user-attachments/assets/1f9ba79e-d110-49f5-b8a0-6c0c6abca9e6)

## 7. Key Resources

Design Theory: Rick DJ0IP's OCFD Presentation (Theory & Construction): https://www.dj0ip.com/hhg2-ocfd

Rope Management: Dale WB6BYU's rope winding technique (invaluable for setup/takedown): https://youtu.be/xmMX6HvunZg?si=jLvIEpQ13_7O2uQT

The whole experience was exhausting but exciting! This antenna is a monster (over 60m long including the support ropes) and best suited for multi-day operations.

73 de Nik SV1SYY
