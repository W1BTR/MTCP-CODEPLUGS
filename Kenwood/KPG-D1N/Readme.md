# Import Into Kenwood KPG-D1N
- [Import Into Kenwood KPG-D1N](#import-into-kenwood-kpg-d1n)
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


### Method 1: Start with .dat file
Using the included MTCP .dat files, begin with this codeplug containing nothing but the MTCP channels and build from there. Great for single-band setups, or to start a multi-band setup.

### Method 2: Copy and Paste from .dat file
You can also open more than one KPG-D1N instance and copy channels over

### Method 3 (Preferred): Copy and Paste Tables Below:
Note that these may be more out of date than the codeplugs. If you have any issues, please report them on the issues page!

Copy one of the below chunks, and paste it into a KPG-D1N Zone (If youre wondering how to make a zone, go in to edit an existing zone, and click "New" in the top left)

# VHF
##### VTAC
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
155.7525	155.7525	Analog	Analog	High	1567	1567	659	659	Narrow	VCALL 10	True	0	255	Common	255
151.1375	151.1375	Analog	Analog	High	1567	1567	659	659	Narrow	VTAC 11	True	0	255	Common	255
154.4525	154.4525	Analog	Analog	High	1567	1567	659	659	Narrow	VTAC 12	True	0	255	Common	255
158.7375	158.7375	Analog	Analog	High	1567	1567	659	659	Narrow	VTAC 13	True	0	255	Common	255
159.4725	159.4725	Analog	Analog	High	1567	1567	659	659	Narrow	VTAC 14	True	0	255	Common	255
159.4725	151.1375	Analog	Analog	High	1567	1365	659	659	Narrow	VTAC 33	True	0	255	Common	255
158.7375	154.4525	Analog	Analog	High	1567	1365	659	659	Narrow	VTAC 34	True	0	255	Common	255
159.4725	158.7375	Analog	Analog	High	1567	1365	659	659	Narrow	VTAC 35	True	0	255	Common	255
151.1375	159.4725	Analog	Analog	High	1567	1365	659	659	Narrow	VTAC 36	True	0	255	Common	255
154.4525	158.7375	Analog	Analog	High	1567	1365	659	659	Narrow	VTAC 37	True	0	255	Common	255
158.7375	159.4725	Analog	Analog	High	1567	1365	659	659	Narrow	VTAC 38	True	0	255	Common	255
```
##### VHF PSC
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
154.28	154.28	Analog	Analog	High	1567	1567	659	659	Narrow	VFIRE21	True	0	255	Common	255
154.265	154.265	Analog	Analog	High	1567	1567	659	659	Narrow	VFIRE22	True	0	255	Common	255
154.295	154.295	Analog	Analog	High	1567	1567	659	659	Narrow	VFIRE23	True	0	255	Common	255
154.2725	154.2725	Analog	Analog	High	1567	1567	659	659	Narrow	VFIRE24	True	0	255	Common	255
154.2875	154.2875	Analog	Analog	High	1567	1567	659	659	Narrow	VFIRE25	True	0	255	Common	255
154.3025	154.3025	Analog	Analog	High	1567	1567	659	659	Narrow	VFIRE26	True	0	255	Common	255
155.475	155.475	Analog	Analog	High	1567	1567	659	659	Narrow	VLAW31	True	0	255	Common	255
155.4825	155.4825	Analog	Analog	High	1567	1567	659	659	Narrow	VLAW32	True	0	255	Common	255
155.34	155.34	Analog	Analog	High	1567	1567	659	659	Narrow	VMED28	True	0	255	Common	255
155.3475	155.3475	Analog	Analog	High	1567	1567	659	659	Narrow	VMED29	True	0	255	Common	255
155.16	155.16	Analog	Analog	High	65535	65535	659	659	Narrow	VSAR16	True	0	255	Common	255
```
##### VHF FED INC RESP
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
169.5375	164.7125	Analog	Analog	High	65535	1679	659	659	Narrow	NC 1	True	0	255	Common	255
170.0125	165.25	Analog	Analog	High	65535	1679	659	659	Narrow	IR 1	True	0	255	Common	255
170.4125	165.9625	Analog	Analog	High	65535	1679	659	659	Narrow	IR 2	True	0	255	Common	255
170.6875	166.575	Analog	Analog	High	65535	1679	659	659	Narrow	IR 3	True	0	255	Common	255
173.0375	167.325	Analog	Analog	High	65535	1679	659	659	Narrow	IR 4	True	0	255	Common	255
169.5375	169.5375	Analog	Analog	High	65535	1679	659	659	Narrow	IR 5	True	0	255	Common	255
170.0125	170.0125	Analog	Analog	High	65535	1679	659	659	Narrow	IR 6	True	0	255	Common	255
170.4125	170.4125	Analog	Analog	High	65535	1679	659	659	Narrow	IR 7	True	0	255	Common	255
170.6875	170.6875	Analog	Analog	High	65535	1679	659	659	Narrow	IR 8	True	0	255	Common	255
173.0375	173.0375	Analog	Analog	High	65535	1679	659	659	Narrow	IR 9	True	0	255	Common	255
```
##### VHF Fed Law
<sup>*Requires P25</sup>
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
##### VHF FIRE DIST
<sup>*Requires P25</sup>
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
##### MARINE 1007-1083
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
156.35	156.35	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1007	True	0	255	Common	255
156.9	156.9	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1018	False	0	255	Common	255
156.95	156.95	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1019	False	0	255	Common	255
157	157	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1020	False	0	255	Common	255
157.05	157.05	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1021	False	0	255	Common	255
157.1	157.1	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1022	False	0	255	Common	255
157.15	157.15	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1023	False	0	255	Common	255
156.175	156.175	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1063	False	0	255	Common	255
156.275	156.275	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1065	False	0	255	Common	255
156.325	156.325	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1066	False	0	255	Common	255
156.925	156.925	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1078	False	0	255	Common	255
156.975	156.975	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1079	False	0	255	Common	255
157.025	157.025	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1080	False	0	255	Common	255
157.075	157.075	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1081	False	0	255	Common	255
157.125	157.125	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1082	False	0	255	Common	255
157.175	157.175	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 1083	True	0	255	Common	255
```
##### MARINE 6-28
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
156.3	156.3	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 6	True	0	255	Common	255
156.4	156.4	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 8	True	0	255	Common	255
156.45	156.45	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 9	True	0	255	Common	255
156.5	156.5	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 10	True	0	255	Common	255
156.55	156.55	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 11	True	0	255	Common	255
156.6	156.6	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 12	False	0	255	Common	255
156.65	156.65	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 13	True	0	255	Common	255
156.7	156.7	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 14	False	0	255	Common	255
156.8	156.8	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 16	False	0	255	Common	255
156.85	156.85	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 17	False	0	255	Common	255
157	157	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 20	False	0	255	Common	255
157.2	157.2	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 24	False	0	255	Common	255
157.25	157.25	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 25	False	0	255	Common	255
157.3	157.3	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 26	False	0	255	Common	255
157.35	157.35	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 27	False	0	255	Common	255
157.4	157.4	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 28	True	0	255	Common	255
```
##### MARINE 67-88
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
156.375	156.375	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 67	True	0	255	Common	255
156.425	156.425	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 68	True	0	255	Common	255
156.475	156.475	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 69	True	0	255	Common	255
156.525	156.525	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 70	True	0	255	Common	255
156.575	156.575	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 71	True	0	255	Common	255
156.625	156.625	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 72	True	0	255	Common	255
156.675	156.675	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 73	True	0	255	Common	255
156.725	156.725	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 74	True	0	255	Common	255
156.875	156.875	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 77	True	0	255	Common	255
157.225	157.225	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 84	True	0	255	Common	255
157.275	157.275	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 85	True	0	255	Common	255
157.325	157.325	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 86	True	0	255	Common	255
157.375	157.375	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 87	True	0	255	Common	255
157.425	157.425	Analog	Analog	High	65535	65535	659	659	Narrow	MARINE CH 88	True	0	255	Common	255
```
##### DCR VHF
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
151.145	151.415	Analog	Analog	High	719	1109	659	659	Narrow	DCR ANDOVER	True	0	255	Common	255
151.145	151.415	Analog	Analog	High	719	1622	659	659	Narrow	DCR BREWSTER	True	0	255	Common	255
151.235	151.235	Analog	Analog	High	719	719	659	659	Narrow	DCR FIRE 13	True	0	255	Common	255
151.145	151.415	Analog	Analog	High	719	719	659	659	Narrow	DCR FIRE 14	True	0	255	Common	255
151.145	151.415	Analog	Analog	High	65535	719	659	659	Narrow	DCR FIREGROUND	True	0	255	Common	255
151.145	151.415	Analog	Analog	High	719	1230	659	659	Narrow	DCR GREYLOCK	True	0	255	Common	255
151.145	151.415	Analog	Analog	High	719	2035	659	659	Narrow	DCR MENDON	True	0	255	Common	255
151.145	151.415	Analog	Analog	High	719	1462	659	659	Narrow	DCR MONTEREY	True	0	255	Common	255
151.145	151.415	Analog	Analog	High	719	948	659	659	Narrow	DCR PELHAM	True	0	255	Common	255
151.145	151.415	Analog	Analog	High	719	1318	659	659	Narrow	DCR PLYMOUTH	True	0	255	Common	255
151.37	151.37	Analog	Analog	High	719	719	659	659	Narrow	DCR REC 15	True	0	255	Common	255
151.145	151.415	Analog	Analog	High	719	825	659	659	Narrow	DCR SHARON	True	0	255	Common	255
151.205	151.205	Analog	Analog	High	719	719	659	659	Narrow	DCR STATEWIDE	True	0	255	Common	255
151.145	151.415	Analog	Analog	High	719	719	659	659	Narrow	DCR WACHUSETT	True	0	255	Common	255
159.285	159.285	Analog	Analog	High	65535	65535	659	659	Narrow	FIRE COMPACT	True	0	255	Common	255
```
##### BRK-HMP-WMLC-D14
```
ZoneChChTableP25ConventionalRxFrequency	ZoneChChTableP25ConventionalTxFrequency	ZoneChChTableP25ConventionalChannelType	ZoneChChTableP25ConventionalTxMode	ZoneChChTableP25ConventionalTxPower	ZoneChChTableP25ConventionalQtDqtDecode	ZoneChChTableP25ConventionalQtDqtEncode	ZoneChChTableP25ConventionalNacDecode	ZoneChChTableP25ConventionalNacEncode	ZoneChChTableP25ConventionalChannelSpacing	ZoneChChTableP25ConventionalChannelName	ZoneChChTableP25ConventionalScanAdd	ZoneChChTableP25ConventionalScanListNo	ZoneChChTableP25ConventionalEmergencyProfileNo	ZoneChChTableP25ConventionalKeyAssignment	ZoneChChTableP25ConventionalVoiceAnnouncement
155.475	155.475	Analog	Analog	High	1738	1738	659	659	Narrow	WM SIM-1 VHF	True	0	255	Common	255
154.28	154.28	Analog	Analog	High	825	825	659	659	Narrow	WM SIM-2 VHF	True	0	255	Common	255
158.8725	158.8725	Analog	Analog	High	1273	1273	659	659	Narrow	HAMPSHIRE TAC1	True	0	255	Common	255
155.34	155.34	Analog	Analog	High	1072	1072	659	659	Narrow	BERK CMED 340	True	0	255	Common	255
154.16	154.16	Analog	Analog	High	1072	1072	659	659	Narrow	BERK FG1	True	0	255	Common	255
158.805	158.805	Analog	Analog	High	1072	1072	659	659	Narrow	BERK FG2	True	0	255	Common	255
153.8825	153.8825	Analog	Analog	High	10467	10467	659	659	Narrow	BERK FG3	True	0	255	Common	255
159.7575	159.7575	Analog	Analog	High	10507	10507	659	659	Narrow	BERK COMMAND	True	0	255	Common	255
154.31	154.31	Analog	Analog	High	1072	1072	659	659	Narrow	BERK DISPATCH	True	0	255	Common	255
155.805	155.805	Analog	Analog	High	1072	1072	659	659	Narrow	BERK INTERIOR	True	0	255	Common	255
152.9825	152.9825	Analog	Analog	High	1318	1318	659	659	Narrow	BERK RESPONSE	True	0	255	Common	255
153.965	153.965	Analog	Analog	High	1072	1072	659	659	Narrow	LAW DISP	True	0	255	Common	255
154.74	154.74	Analog	Analog	High	1072	1072	659	659	Narrow	LAW TAC 1	True	0	255	Common	255
154.74	159	Analog	Analog	High	10506	10515	659	659	Narrow	PD CMD RPTR	True	0	255	Common	255
159.045	159.045	Analog	Analog	High	10316	10316	659	659	Narrow	14 SILVER	True	0	255	Common	255
```
##### MEMA
<sup>*Requires P25</sup>
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