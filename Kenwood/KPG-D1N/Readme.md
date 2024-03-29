# Import Into Kenwood KPG-D1N
- [Import Into Kenwood KPG-D1N](#import-into-kenwood-kpg-d1n)
      - [This codeplug currently has an issue where some VHF zones that should be in analog systems are in Digital / P25 systems](#this-codeplug-currently-has-an-issue-where-some-vhf-zones-that-should-be-in-analog-systems-are-in-digital--p25-systems)
    - [Method 1: Start with .dat file](#method-1-start-with-dat-file)
    - [Method 2: Copy and Paste from .dat file](#method-2-copy-and-paste-from-dat-file)
    - [Method 3 (Preferred): Copy and Paste Tables Below:](#method-3-preferred-copy-and-paste-tables-below)
- [VHF](#vhf)
        - [VTAC](#vtac)
        - [VHF PSC](#vhf-psc)
        - [VHF FED INC RESP](#vhf-fed-inc-resp)
        - [VHF Fed Law](#vhf-fed-law)
        - [VHF FIRE DIST](#vhf-fire-dist)
        - [MARINE 1007-1083](#marine-1007-1083)
        - [MARINE 6-28](#marine-6-28)
        - [MARINE 67-88](#marine-67-88)
        - [DCR VHF](#dcr-vhf)
        - [BRK-HMP-WMLC-D14](#brk-hmp-wmlc-d14)
        - [MEMA](#mema)
- [UHF](#uhf)
        - [UHF NON FED INTEROP (UTAC) ANALOG](#uhf-non-fed-interop-utac-analog)
        - [UHF FED INC RESP (FED IR U) ANALOG](#uhf-fed-inc-resp-fed-ir-u-analog)


### Method 1: Start with .dat file
Using the included MTCP .dat files, begin with this codeplug containing nothing but the MTCP channels and build from there. Great for single-band setups, or to start a multi-band setup.

### Method 2: Copy and Paste from .dat file
You can also open more than one KPG-D1N instance and copy channels over

### Method 3 (Preferred): Copy and Paste Tables Below:
Note that these may be more out of date than the codeplugs. If you have any issues, please report them on the issues page!

1. Create a KPG-D1N Codeplug for your radio
2. After creating the zones you'd like for your municipality, **create a new zone** for each of the below required zones that are within the TX/RX range of your radio (If youre wondering how to make a zone, go in to edit an existing zone, and click "New" in the top left).
3. Make sure to **set the system** to an analog one for chunks with <sup>ANALOG</sup> marked on them, and P25 Conventional for chunks labeled <sup>P25</sup> (this is done in `PERSONAL -> SYSTEM -> SYSTEM INFORMATION`)
4. **Copy the chunk** of code for the zone, select one fo the cells in KPG-D1N, and **paste** it.
5. Rinse and repeat!


# VHF
##### VTAC <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
155.7525	155.7525	Analog	High	1567	1567	Narrow	VCALL 10	True	0	255	Common	255
151.1375	151.1375	Analog	High	1567	1567	Narrow	VTAC 11	True	0	255	Common	255
154.4525	154.4525	Analog	High	1567	1567	Narrow	VTAC 12	True	0	255	Common	255
158.7375	158.7375	Analog	High	1567	1567	Narrow	VTAC 13	True	0	255	Common	255
159.4725	159.4725	Analog	High	1567	1567	Narrow	VTAC 14	True	0	255	Common	255
159.4725	151.1375	Analog	High	1567	1365	Narrow	VTAC 33	True	0	255	Common	255
158.7375	154.4525	Analog	High	1567	1365	Narrow	VTAC 34	True	0	255	Common	255
159.4725	158.7375	Analog	High	1567	1365	Narrow	VTAC 35	True	0	255	Common	255
151.1375	159.4725	Analog	High	1567	1365	Narrow	VTAC 36	True	0	255	Common	255
154.4525	158.7375	Analog	High	1567	1365	Narrow	VTAC 37	True	0	255	Common	255
158.7375	159.4725	Analog	High	1567	1365	Narrow	VTAC 38	True	0	255	Common	255

```
##### VHF PSC <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
154.28	154.28	Analog	High	1567	1567	Narrow	VFIRE21	True	0	255	Common	255
154.265	154.265	Analog	High	1567	1567	Narrow	VFIRE22	True	0	255	Common	255
154.295	154.295	Analog	High	1567	1567	Narrow	VFIRE23	True	0	255	Common	255
154.2725	154.2725	Analog	High	1567	1567	Narrow	VFIRE24	True	0	255	Common	255
154.2875	154.2875	Analog	High	1567	1567	Narrow	VFIRE25	True	0	255	Common	255
154.3025	154.3025	Analog	High	1567	1567	Narrow	VFIRE26	True	0	255	Common	255
155.475	155.475	Analog	High	1567	1567	Narrow	VLAW31	True	0	255	Common	255
155.4825	155.4825	Analog	High	1567	1567	Narrow	VLAW32	True	0	255	Common	255
155.34	155.34	Analog	High	1567	1567	Narrow	VMED28	True	0	255	Common	255
155.3475	155.3475	Analog	High	1567	1567	Narrow	VMED29	True	0	255	Common	255
155.16	155.16	Analog	High	65535	65535	Narrow	VSAR16	True	0	255	Common	255
```
##### VHF FED INC RESP <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
169.5375	164.7125	Analog	High	65535	1679	Narrow	NC 1	True	0	255	Common	255
170.0125	165.25	Analog	High	65535	1679	Narrow	IR 1	True	0	255	Common	255
170.4125	165.9625	Analog	High	65535	1679	Narrow	IR 2	True	0	255	Common	255
170.6875	166.575	Analog	High	65535	1679	Narrow	IR 3	True	0	255	Common	255
173.0375	167.325	Analog	High	65535	1679	Narrow	IR 4	True	0	255	Common	255
169.5375	169.5375	Analog	High	65535	1679	Narrow	IR 5	True	0	255	Common	255
170.0125	170.0125	Analog	High	65535	1679	Narrow	IR 6	True	0	255	Common	255
170.4125	170.4125	Analog	High	65535	1679	Narrow	IR 7	True	0	255	Common	255
170.6875	170.6875	Analog	High	65535	1679	Narrow	IR 8	True	0	255	Common	255
173.0375	173.0375	Analog	High	65535	1679	Narrow	IR 9	True	0	255	Common	255
```
##### VHF FED LAW <SUP>P25</SUP>
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
167.0875	167.0875	Analog	Analog	High	65535	1679	659	659	Narrow	LE A	True	0	255	Common	255
167.0875	162.0875	Analog	Analog	High	65535	1679	659	659	Narrow	LE 1	False	0	255	Common	255
167.25	162.2625	P25	P25	High	65535	65535	1679	1679	Narrow	LE 2	False	0	255	Common	255
167.75	162.8375	P25	P25	High	65535	65535	1679	1679	Narrow	LE 3	False	0	255	Common	255
168.1125	163.2875	P25	P25	High	65535	65535	1679	1679	Narrow	LE 4	False	0	255	Common	255
168.4625	163.425	P25	P25	High	65535	65535	1679	1679	Narrow	LE 5	False	0	255	Common	255
167.25	167.25	P25	P25	High	65535	65535	1679	1679	Narrow	LE 6	False	0	255	Common	255
167.75	167.75	P25	P25	High	65535	65535	1679	1679	Narrow	LE 7	False	0	255	Common	255
168.1125	168.1125	P25	P25	High	65535	65535	1679	1679	Narrow	LE 8	False	0	255	Common	255
168.4625	168.4625	P25	P25	High	65535	65535	1679	1679	Narrow	LE 9	False	0	255	Common	255
```
##### VHF FIRE DIST <SUP>P25</SUP>
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
155.7225	158.94	P25	P25	High	65535	65535	553	1424	Narrow	DUK FD-TAC	True	0	255	Common	255
154.355	154.355	Analog	Analog	High	1148	1148	659	659	Narrow	DUK FG1	False	0	255	Common	255
154.415	154.415	Analog	Analog	High	1148	1148	659	659	Narrow	DUK FG2	False	0	255	Common	255
154.07	154.07	Analog	Analog	High	1148	1148	659	659	Narrow	DUK FG3	False	0	255	Common	255
154.385	154.385	Analog	Analog	High	1148	1148	659	659	Narrow	DUK FG4	False	0	255	Common	255
155.925	159.345	P25	P25	High	65535	65535	3344	3408	Narrow	DUK OPS-DN	False	0	255	Common	255
151.265	158.82	P25	P25	High	65535	65535	3344	3408	Narrow	DUK OPS-EN	False	0	255	Common	255
154.8225	159.135	P25	P25	High	65535	65535	3344	3408	Narrow	DUK OPS-UP	False	0	255	Common	255
153.83	153.83	Analog	Analog	High	65535	770	659	659	Narrow	FD5 EC RED V	False	0	255	Common	255
154.28	154.28	Analog	Analog	High	1365	1365	659	659	Narrow	FD5 EC WHITE	False	0	255	Common	255
154.07	158.73	Analog	Analog	High	1318	10390	659	659	Narrow	FIRE FIST 5 V	False	0	255	Common	255
154.07	158.73	Analog	Analog	High	1318	10467	659	659	Narrow	FIRE FIST 15 V	False	0	255	Common	255
153.83	153.83	Analog	Analog	High	770	770	659	659	Narrow	FD6 FG1 V	False	0	255	Common	255
154.295	154.295	Analog	Analog	High	744	744	659	659	Narrow	D7 BLUE	False	0	255	Common	255
159.4575	151.2725	Analog	Analog	High	915	915	659	659	Narrow	D7 ORANGE	False	0	255	Common	255
154.265	154.265	Analog	Analog	High	744	744	659	659	Narrow	D7 RED	True	0	255	Common	255
```
##### MARINE 1007-1083 <SUP>ANALOG</SUP>
```

ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
156.35	156.35	Analog	High	65535	65535	Narrow	MARINE CH 1007	True	0	255	Common	255
156.9	156.9	Analog	High	65535	65535	Narrow	MARINE CH 1018	True	0	255	Common	255
156.95	156.95	Analog	High	65535	65535	Narrow	MARINE CH 1019	True	0	255	Common	255
157	157	Analog	High	65535	65535	Narrow	MARINE CH 1020	True	0	255	Common	255
157.05	157.05	Analog	High	65535	65535	Narrow	MARINE CH 1021	True	0	255	Common	255
157.1	157.1	Analog	High	65535	65535	Narrow	MARINE CH 1022	True	0	255	Common	255
157.15	157.15	Analog	High	65535	65535	Narrow	MARINE CH 1023	True	0	255	Common	255
156.175	156.175	Analog	High	65535	65535	Narrow	MARINE CH 1063	True	0	255	Common	255
156.275	156.275	Analog	High	65535	65535	Narrow	MARINE CH 1065	True	0	255	Common	255
156.325	156.325	Analog	High	65535	65535	Narrow	MARINE CH 1066	True	0	255	Common	255
156.925	156.925	Analog	High	65535	65535	Narrow	MARINE CH 1078	True	0	255	Common	255
156.975	156.975	Analog	High	65535	65535	Narrow	MARINE CH 1079	True	0	255	Common	255
157.025	157.025	Analog	High	65535	65535	Narrow	MARINE CH 1080	True	0	255	Common	255
157.075	157.075	Analog	High	65535	65535	Narrow	MARINE CH 1081	True	0	255	Common	255
157.125	157.125	Analog	High	65535	65535	Narrow	MARINE CH 1082	True	0	255	Common	255
157.175	157.175	Analog	High	65535	65535	Narrow	MARINE CH 1083	True	0	255	Common	255

```
##### MARINE 6-28 <SUP>ANALOG</SUP>
```

ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
156.3	156.3	Analog	High	65535	65535	Narrow	MARINE CH 6	True	0	255	Common	255
156.4	156.4	Analog	High	65535	65535	Narrow	MARINE CH 8	False	0	255	Common	255
156.45	156.45	Analog	High	65535	65535	Narrow	MARINE CH 9	False	0	255	Common	255
156.5	156.5	Analog	High	65535	65535	Narrow	MARINE CH 10	False	0	255	Common	255
156.55	156.55	Analog	High	65535	65535	Narrow	MARINE CH 11	False	0	255	Common	255
156.6	156.6	Analog	High	65535	65535	Narrow	MARINE CH 12	False	0	255	Common	255
156.65	156.65	Analog	High	65535	65535	Narrow	MARINE CH 13	False	0	255	Common	255
156.7	156.7	Analog	High	65535	65535	Narrow	MARINE CH 14	False	0	255	Common	255
156.8	156.8	Analog	High	65535	65535	Narrow	MARINE CH 16	False	0	255	Common	255
156.85	156.85	Analog	High	65535	65535	Narrow	MARINE CH 17	False	0	255	Common	255
157	157	Analog	High	65535	65535	Narrow	MARINE CH 20	True	0	255	Common	255
157.2	157.2	Analog	High	65535	65535	Narrow	MARINE CH 24	True	0	255	Common	255
157.25	157.25	Analog	High	65535	65535	Narrow	MARINE CH 25	True	0	255	Common	255
157.3	157.3	Analog	High	65535	65535	Narrow	MARINE CH 26	True	0	255	Common	255
157.35	157.35	Analog	High	65535	65535	Narrow	MARINE CH 27	True	0	255	Common	255
157.4	157.4	Analog	High	65535	65535	Narrow	MARINE CH 28	True	0	255	Common	255


```
##### MARINE 67-88 <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
156.375	156.375	Analog	High	65535	65535	Narrow	MARINE CH 67	True	0	255	Common	255
156.425	156.425	Analog	High	65535	65535	Narrow	MARINE CH 68	True	0	255	Common	255
156.475	156.475	Analog	High	65535	65535	Narrow	MARINE CH 69	True	0	255	Common	255
156.525	156.525	Analog	High	65535	65535	Narrow	MARINE CH 70	True	0	255	Common	255
156.575	156.575	Analog	High	65535	65535	Narrow	MARINE CH 71	True	0	255	Common	255
156.625	156.625	Analog	High	65535	65535	Narrow	MARINE CH 72	True	0	255	Common	255
156.675	156.675	Analog	High	65535	65535	Narrow	MARINE CH 73	True	0	255	Common	255
156.725	156.725	Analog	High	65535	65535	Narrow	MARINE CH 74	True	0	255	Common	255
156.875	156.875	Analog	High	65535	65535	Narrow	MARINE CH 77	True	0	255	Common	255
157.225	157.225	Analog	High	65535	65535	Narrow	MARINE CH 84	True	0	255	Common	255
157.275	157.275	Analog	High	65535	65535	Narrow	MARINE CH 85	True	0	255	Common	255
157.325	157.325	Analog	High	65535	65535	Narrow	MARINE CH 86	True	0	255	Common	255
157.375	157.375	Analog	High	65535	65535	Narrow	MARINE CH 87	True	0	255	Common	255
157.425	157.425	Analog	High	65535	65535	Narrow	MARINE CH 88	True	0	255	Common	255
```
##### DCR VHF <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
151.145	151.415	Analog	High	719	1109	Narrow	DCR ANDOVER	True	0	255	Common	255
151.145	151.415	Analog	High	719	1622	Narrow	DCR BREWSTER	True	0	255	Common	255
151.235	151.235	Analog	High	719	719	Narrow	DCR FIRE 13	True	0	255	Common	255
151.145	151.415	Analog	High	719	719	Narrow	DCR FIRE 14	True	0	255	Common	255
151.145	151.415	Analog	High	65535	719	Narrow	DCR FIREGROUND	True	0	255	Common	255
151.145	151.415	Analog	High	719	1230	Narrow	DCR GREYLOCK	True	0	255	Common	255
151.145	151.415	Analog	High	719	2035	Narrow	DCR MENDON	True	0	255	Common	255
151.145	151.415	Analog	High	719	1462	Narrow	DCR MONTEREY	True	0	255	Common	255
151.145	151.415	Analog	High	719	948	Narrow	DCR PELHAM	True	0	255	Common	255
151.145	151.415	Analog	High	719	1318	Narrow	DCR PLYMOUTH	True	0	255	Common	255
151.37	151.37	Analog	High	719	719	Narrow	DCR REC 15	True	0	255	Common	255
151.145	151.415	Analog	High	719	825	Narrow	DCR SHARON	True	0	255	Common	255
151.205	151.205	Analog	High	719	719	Narrow	DCR STATEWIDE	True	0	255	Common	255
151.145	151.415	Analog	High	719	719	Narrow	DCR WACHUSETT	True	0	255	Common	255
159.285	159.285	Analog	High	65535	65535	Narrow	FIRE COMPACT	True	0	255	Common	255
```
##### BRK-HMP-WMLC-D14 <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
155.475	155.475	Analog	High	1738	1738	Narrow	WM SIM-1 VHF	True	0	255	Common	255
154.28	154.28	Analog	High	825	825	Narrow	WM SIM-2 VHF	True	0	255	Common	255
158.8725	158.8725	Analog	High	1273	1273	Narrow	HAMPSHIRE TAC1	True	0	255	Common	255
155.34	155.34	Analog	High	1072	1072	Narrow	BERK CMED 340	True	0	255	Common	255
154.16	154.16	Analog	High	1072	1072	Narrow	BERK FG1	True	0	255	Common	255
158.805	158.805	Analog	High	1072	1072	Narrow	BERK FG2	True	0	255	Common	255
153.8825	153.8825	Analog	High	10467	10467	Narrow	BERK FG3	True	0	255	Common	255
159.7575	159.7575	Analog	High	10507	10507	Narrow	BERK COMMAND	True	0	255	Common	255
154.31	154.31	Analog	High	1072	1072	Narrow	BERK DISPATCH	True	0	255	Common	255
155.805	155.805	Analog	High	1072	1072	Narrow	BERK INTERIOR	True	0	255	Common	255
152.9825	152.9825	Analog	High	1318	1318	Narrow	BERK RESPONSE	True	0	255	Common	255
153.965	153.965	Analog	High	1072	1072	Narrow	LAW DISP	True	0	255	Common	255
154.74	154.74	Analog	High	1072	1072	Narrow	LAW TAC 1	True	0	255	Common	255
154.74	159	Analog	High	10506	10515	Narrow	PD CMD RPTR	True	0	255	Common	255
159.045	159.045	Analog	High	10316	10316	Narrow	14 SILVER	True	0	255	Common	255
```
##### MEMA <SUP>P25</SUP>
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
151.2575	154.785	Analog	Analog	High	10505	10533	659	659	Narrow	R1 AMESBURY	True	0	255	Common	255
153.965	154.785	Analog	Analog	High	2035	10533	659	659	Narrow	R1 BOSTON	True	0	255	Common	255
155.745	154.785	Analog	Analog	High	1000	10533	659	659	Narrow	R1 FRAMINGHAM	True	0	255	Common	255
155.4375	154.785	Analog	Analog	High	10586	10533	659	659	Narrow	R1 TEWKSBURY	True	0	255	Common	255
154.7475	156.135	Analog	Analog	High	10349	10586	659	659	Narrow	R2 BRIDGEWATER	True	0	255	Common	255
154.085	156.135	Analog	Analog	High	2107	10586	659	659	Narrow	R2 PLYMOUTH	True	0	255	Common	255
155.085	155.955	Analog	Analog	High	2257	10349	659	659	Narrow	R3 ADAMS	True	0	255	Common	255
153.905	155.955	Analog	Analog	High	10586	10349	659	659	Narrow	R3 PELHAM	True	0	255	Common	255
151.4525	155.955	Analog	Analog	High	2291	10349	659	659	Narrow	R3 PRINCETON	True	0	255	Common	255
154.8225	154.8225	Analog	Analog	High	10390	10390	659	659	Narrow	SW TACTICAL	True	0	255	Common	255
158.91	154.86	Analog	Analog	High	10634	10357	659	659	Narrow	BPD FED IO	True	0	255	Common	255
154.175	159.06	P25	P25	High	65535	65535	1542	354	Narrow	BPD MEDIC	True	0	255	Common	255
```
# UHF

##### UHF NON FED INTEROP (UTAC) <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
453.2125	458.2125	Analog	High	1567	1567	Narrow	UCALL 40	True	0	255	Common	255
453.2125	453.2125	Analog	High	1567	1567	Narrow	UCALL 40 D	True	0	255	Common	255
453.4625	458.4625	Analog	High	1567	1567	Narrow	UTAC 41	True	0	255	Common	255
453.4625	453.4625	Analog	High	1567	1567	Narrow	UTAC 41 D	True	0	255	Common	255
453.7125	458.7125	Analog	High	1567	1567	Narrow	UTAC 42	True	0	255	Common	255
453.7125	453.7125	Analog	High	1567	1567	Narrow	UTAC 42 D	True	0	255	Common	255
453.8625	458.8625	Analog	High	1567	1567	Narrow	UTAC 43	True	0	255	Common	255
453.8625	453.8625	Analog	High	1567	1567	Narrow	UTAC 43 D	True	0	255	Common	255
```
##### UHF FED INC RESP (FED IR U) <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
410.2375	419.2375	Analog	High	65535	1679	Narrow	NC 2	True	0	255	Common	255
410.4375	419.475	Analog	High	65535	1679	Narrow	IR 10	True	0	255	Common	255
410.6375	419.6375	Analog	High	65535	1679	Narrow	IR 11	True	0	255	Common	255
410.8375	419.8375	Analog	High	65535	1679	Narrow	IR 12	True	0	255	Common	255
413.1875	413.1875	Analog	High	65535	1679	Narrow	IR 13	True	0	255	Common	255
413.2125	413.2125	Analog	High	65535	1679	Narrow	IR 14	True	0	255	Common	255
410.2375	410.2375	Analog	High	65535	1679	Narrow	IR 15	True	0	255	Common	255
410.4375	410.4375	Analog	High	65535	1679	Narrow	IR 16	True	0	255	Common	255
410.6375	410.6375	Analog	High	65535	1679	Narrow	IR 17	True	0	255	Common	255
410.8375	410.8375	Analog	High	65535	1679	Narrow	IR 18	True	0	255	Common	255
```
##### UHF FED LAW (FED LE U) <SUP>P25</SUP>
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
414.0375	414.0375	Analog	Analog	High	65535	1679	659	659	Narrow	LE B	True	0	255	Common	255
409.9875	418.9875	Analog	Analog	High	65535	1679	659	659	Narrow	LE 10	True	0	255	Common	255
410.1875	418.1875	P25	P25	High	65535	65535	1679	1679	Narrow	LE 11	True	0	255	Common	255
410.6125	419.6125	P25	P25	High	65535	65535	1679	1679	Narrow	LE 12	True	0	255	Common	255
414.0625	414.0625	P25	P25	High	65535	65535	1679	1679	Narrow	LE 13	True	0	255	Common	255
414.3125	414.3125	P25	P25	High	65535	65535	1679	1679	Narrow	LE 14	True	0	255	Common	255
414.3375	414.3375	P25	P25	High	65535	65535	1679	1679	Narrow	LE 15	True	0	255	Common	255
409.9875	409.9875	Analog	Analog	High	65535	1679	659	659	Narrow	LE 16	True	0	255	Common	255
410.1875	410.1875	P25	P25	High	65535	65535	1679	1679	Narrow	LE 17	True	0	255	Common	255
410.6125	410.6125	P25	P25	High	65535	65535	1679	1679	Narrow	LE 18	True	0	255	Common	255
```
##### BAPERN (BAPERN, BUT SMALLER) <SUP>P25</SUP>
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
470.7875	470.7875	Analog	Analog	High	1318	10403	659	659	Narrow	AREAWIDE 3	True	0	255	Common	255
470.5625	470.5625	Analog	Analog	High	1318	10404	659	659	Narrow	AREAWIDE 4	True	0	255	Common	255
470.9875	470.9875	Analog	Analog	High	10668	10387	659	659	Narrow	BAP CENT DIST	True	0	255	Common	255
470.0375	470.0375	P25	P25	High	65535	65535	1634	550	Narrow	BAP CENT TAC	True	0	255	Common	255
470.4875	470.4875	Analog	Analog	High	1318	10405	659	659	Narrow	BAP NORTH DIST	True	0	255	Common	255
482.9625	482.9625	P25	P25	High	65535	65535	1335	1335	Narrow	BAP NORTH TAC	True	0	255	Common	255
482.6875	482.6875	Analog	Analog	High	1462	10419	659	659	Narrow	BAP NW DIST	True	0	255	Common	255
482.6375	482.6375	P25	P25	High	65535	65535	1335	1335	Narrow	BAP NW TAC	True	0	255	Common	255
482.8875	482.8875	Analog	Analog	High	2035	10421	659	659	Narrow	BAP SE DIST	True	0	255	Common	255
483.0375	483.0375	P25	P25	High	65535	65535	1335	1335	Narrow	BAP SE TAC	True	0	255	Common	255
470.9125	470.9125	Analog	Analog	High	1318	10409	659	659	Narrow	BAP SOUTH DIST	True	0	255	Common	255
470.15	470.15	P25	P25	High	65535	65535	1575	370	Narrow	BAP SOUTH TAC	True	0	255	Common	255
482.5125	482.5125	Analog	Analog	High	2035	2035	659	659	Narrow	BAP SW DIST	True	0	255	Common	255
470.7375	470.7375	Analog	Analog	High	1318	10417	659	659	Narrow	BAP WEST DIST	True	0	255	Common	255
470.075	470.075	P25	P25	High	65535	65535	152	100	Narrow	BAP WEST TAC	True	0	255	Common	255
```
##### BERKSHIRE UHF (BERK UHF) <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
465.375	465.375	Analog	High	10549	10549	Narrow	Channel 1	True	0	255	Common	255
465.625	465.625	Analog	High	10563	10563	Narrow	Channel 2	True	0	255	Common	255
453.6125	458.6125	Analog	High	10586	10586	Narrow	Channel 3	True	0	255	Common	255
460.0625	465.0625	Analog	High	10613	10613	Narrow	Channel 4	True	0	255	Common	255
460.575	465.575	Analog	High	10630	10630	Narrow	Channel 5	True	0	255	Common	255
453.65	458.65	Analog	High	10649	10649	Narrow	Channel 6	True	0	255	Common	255
453.45	453.45	Analog	High	10329	10329	Narrow	Channel 7	True	0	255	Common	255
458.4375	458.4375	Analog	High	10350	10350	Narrow	Channel 8	True	0	255	Common	255
458.45	458.45	Analog	High	10362	10362	Narrow	Channel 9	True	0	255	Common	255
460.0375	460.0375	Analog	High	10403	10403	Narrow	Channel 10	True	0	255	Common	255
460.2	460.2	Analog	High	10438	10438	Narrow	Channel 11	True	0	255	Common	255
460.375	460.375	Analog	High	10457	10457	Narrow	Channel 12	True	0	255	Common	255
460.625	460.625	Analog	High	10484	10484	Narrow	Channel 13	True	0	255	Common	255
465.0375	465.0375	Analog	High	10505	10505	Narrow	Channel 14	True	0	255	Common	255
465.2	465.2	Analog	High	10521	10521	Narrow	Channel 15	True	0	255	Common	255
460.3875	465.3875	Analog	High	1072	1072	Narrow	Channel 16	True	0	255	Common	255

```
##### WMLEC UHF (WMLEC U) <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
453.1	458.1	Analog	High	2065	2065	Narrow	WM BORDEN 1	True	0	255	Common	255
453.4125	458.4125	Analog	High	2065	2065	Narrow	WM BORDEN 2	True	0	255	Common	255
453.15	458.15	Analog	High	2065	2065	Narrow	WM GRACE 1	True	0	255	Common	255
453.6	458.6	Analog	High	2065	2065	Narrow	WM GRACE 2	True	0	255	Common	255
453.475	458.475	Analog	High	2065	2065	Narrow	WM SHELBURNE 1	True	0	255	Common	255
453.8	458.8	Analog	High	2065	2065	Narrow	WM SHELBURNE 2	True	0	255	Common	255
460.25	465.25	Analog	High	2065	2065	Narrow	WM HOVEY 1	True	0	255	Common	255
460.625	465.625	Analog	High	2065	2065	Narrow	WM HOVEY 2	True	0	255	Common	255
453.9	458.9	Analog	High	2065	2065	Narrow	WM MT TOM 1	True	0	255	Common	255
452.5875	457.5875	Analog	High	2065	2065	Narrow	WM MT TOM 2	True	0	255	Common	255
460.225	465.225	Analog	High	2065	2065	Narrow	WM SIM 1A	True	0	255	Common	255
460.475	465.475	Analog	High	2065	2065	Narrow	WM SIM 2A	True	0	255	Common	255
```
##### FD DIST 6-8-14 (FD6-8-14) <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
486.6375	486.6375	Analog	High	10390	10390	Narrow	FD6 FG1 U	True	0	255	Common	255
483.6375	483.6375	Analog	High	1567	1567	Narrow	FD6 FG2	True	0	255	Common	255
484.3875	484.3875	Analog	High	10304	10304	Narrow	FD6 FG3	True	0	255	Common	255
483.6375	486.6375	Analog	High	1567	1567	Narrow	FD6 ADMIN	True	0	255	Common	255
460.0375	465.0375	Analog	High	1318	1318	Narrow	FD6 OPS	True	0	255	Common	255
453.75	458.75	Analog	High	948	948	Narrow	FD8 SIMULCAST	True	0	255	Common	255
453.9125	453.9125	Analog	High	1318	1318	Narrow	FD8 RED	True	0	255	Common	255
458.9625	458.9625	Analog	High	1318	1318	Narrow	FD8 WHITE	True	0	255	Common	255
453.9875	453.9875	Analog	High	1318	1318	Narrow	FD8 BLUE	True	0	255	Common	255
453.5375	453.5375	Analog	High	1188	1188	Narrow	14 BLUE	True	0	255	Common	255
460.1	465.1	Analog	High	744	744	Narrow	14 GOLD	True	0	255	Common	255
453.3875	453.3875	Analog	High	10293	10293	Narrow	14 GREEN	True	0	255	Common	255
453.5375	458.5375	Analog	High	10293	10293	Narrow	14 ORANGE	True	0	255	Common	255
460.1	460.1	Analog	High	744	744	Narrow	14 RED	True	0	255	Common	255
471.05	471.05	Analog	High	10362	10362	Narrow	14 WHITE	True	0	255	Common	255
```
##### METRO FIRE D13 (METRO 13) <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
482.025	482.025	Analog	High	65535	65535	Narrow	CENTRAL DIRECT	True	0	255	Common	255
482.025	485.025	Analog	High	65535	65535	Narrow	CENTRAL DIST	True	0	255	Common	255
485.1875	485.1875	Analog	High	65535	65535	Narrow	CENTRAL FG	True	0	255	Common	255
483.3125	485.1875	Analog	High	65535	65535	Narrow	METRO RED	True	0	255	Common	255
482.25	482.25	Analog	High	65535	65535	Narrow	NORTH DIRECT	True	0	255	Common	255
482.25	485.25	Analog	High	65535	65535	Narrow	NORTH DIST	True	0	255	Common	255
482.1875	482.1875	Analog	High	65535	65535	Narrow	NORTH FG	True	0	255	Common	255
470.1875	473.1875	Analog	High	65535	65535	Narrow	ORANGE	True	0	255	Common	255
483.3125	486.3125	Analog	High	65535	65535	Narrow	RED	True	0	255	Common	255
483.3125	483.3125	Analog	High	65535	65535	Narrow	RED DIR	True	0	255	Common	255
470.1375	473.1375	Analog	High	65535	65535	Narrow	SILVER	True	0	255	Common	255
482.2125	482.2125	Analog	High	65535	65535	Narrow	SOUTH DIRECT	True	0	255	Common	255
482.2125	485.2125	Analog	High	65535	65535	Narrow	SOUTH DIST	True	0	255	Common	255
485.1	485.1	Analog	High	65535	65535	Narrow	SOUTH FG	True	0	255	Common	255
```
##### MBHSR-MPA (MBHSRMPA) <SUP>ANALOG</SUP>
```
ZoneChChTableAnalogConventionalRxFrequency	ZoneChChTableAnalogConventionalTxFrequency	ZoneChChTableAnalogConventionalTxMode	ZoneChChTableAnalogConventionalTxPower	ZoneChChTableAnalogConventionalQtDqtDecode	ZoneChChTableAnalogConventionalQtDqtEncode	ZoneChChTableAnalogConventionalChannelSpacingAnalog	ZoneChChTableAnalogConventionalChannelName	ZoneChChTableAnalogConventionalScanAdd	ZoneChChTableAnalogConventionalScanListNo	ZoneChChTableAnalogConventionalEmergencyProfileNo	ZoneChChTableAnalogConventionalKeyAssignment	ZoneChChTableAnalogConventionalVoiceAnnouncement
453.9	458.9	Analog	High	10373	10373	Narrow	MASSPORT UHF	True	0	255	Common	255
453.9	458.9	Analog	High	10373	10373	Narrow	MPA-FD1 UHF	True	0	255	Common	255
460.6375	465.6375	Analog	High	10485	10390	Narrow	MPA-FD5 UHF	True	0	255	Common	255
470.0125	473.0125	Analog	High	1273	10674	Narrow	MBHSR	True	0	255	Common	255
470.2	473.2	Analog	High	1035	1318	Narrow	REGIONAL RPT	True	0	255	Common	255
470.2	470.2	Analog	High	1035	1035	Narrow	REGIONAL TAC 1	True	0	255	Common	255
473.2	473.2	Analog	High	1072	1072	Narrow	REGIONAL TAC 2	True	0	255	Common	255
453.1	458.1	Analog	High	10357	10357	Narrow	BAMA	True	0	255	Common	255
462.9625	462.9625	Analog	High	885	885	Narrow	SOPS MED92 DIR	True	0	255	Common	255
471.6875	474.6875	Analog	High	10630	10354	Narrow	MEMA TIE UHF	True	0	255	Common	255
```