# Ra-07H_LoRa_868


Ra-07H

# Settings

COM9

Default: 115200

---

AT

ASR6501/ASR6502 AT Command 

manufacturer identification
```
AT+CGMI?
```

model identification
```
AT+CGMM?
```

revision identification
```
AT+CGMR?
```

product serial number identification
```
AT+CGSN?
```

baud rate on UART interface
```
AT+CGBR?
```

Set/Read Join Mode +CJOINMODE
```
AT+CJOINMODE?
```

Set/Read DevEUI +CDEVEUI
```
AT+CDEVEUI?
```

Set/Read DevAddr +CDEVADDR
```
AT+CDEVADDR?
```

Set Frequency Band Mask +CFREQBANDMASK
```
AT+CFREQBANDMASK?
```

Set/Read Upload/Download Same/Different Frequency +CULDLMODE
```
AT+CULDLMODE?
```

Set/Read Class +CCLASS
```
AT+CCLASS?
```

Inquire the Battery level of Device Node +CBL
```
AT+CBL?
```

Inquire Device Current Status +CSTATUS
```
AT+CSTATUS?
```

Send/Receive +DTRX
```
AT+DTRX=?

//example
AT+DTRX=1,2,10,0123456789
OK+SEND:03
OK+SENT:01
OK+RECV:02,01,00
```

Receive Data +DRX
```
AT+DRX?
```

```
AT+CRSSI FREQBANDIDX?
```

Sets or reads the receive window parameters +CRXP
```
AT+CRXP?

//example
ASR6501:~# AT+CRXP?
+CRXP:0,0,869525000
OK

```

Restart Module +IREBOOT
```
0 ：Restart the communication module immediately
1 ：Wait for the wireless frame currently being sent in the

AT+IREBOOT=0
```

Setting the Log Level +ILOGLVL
```
AT+ILOGLVL?
```

```

```

# Sleep

AT+CSLEEP=?

+CSLEEP = <0, 1, 2 >
OK

AT+CSLEEP=<sleep_mode>

0 – 进入DeepSleep模式，并于10s后由Timer
1 – 进入DeepSleep模式，并由set_b
2 – 进入DeepSleep模式，并由UART

Baud

AT+CGBR?

AT+CGBR=<baud>

AT+CGBR=9600 OK


---



Following table-1 lists out LoRa frequency channels in 868 MHz Band.

The band is from 863 to 870 MHz. It mentions channel number and its respective channel frequency. 

All the 8 channels are separated by 0.3 MHz with respect to the adjacent channels.

| Channel Number  | LoRa Center Frequency |
| :------------ | :------------ |
|CH_10_868 |865.20 MHz |
|CH_11_868 |865.50 MHz |
|CH_12_868 |865.80 MHz |
|CH_13_868 |866.10 MHz |
|CH_14_868 |866.40 MHz |
|CH_15_868 |866.70 MHz |
|CH_16_868 |867 MHz |
|CH_17_868 |868 MHz |

Following table-2 lists out LoRa channels in 900 MHz Band.

The band is from 902 to 928 MHz.
 
It mentions channel number and its respective channel frequency.
  
All the 13 channels are separated by 2.16 MHz with respect to the adjacent channels.

| Channel Number  | LoRa Center Frequency |
| :------------ | :------------ |
|CH_00_900 |903.08 MHz |
|CH_01_900 |905.24 MHz |
|CH_02_900 |907.40 MHz |
|CH_03_900 |909.56 MHz |
|CH_04_900 |911.72 MHz |
|CH_05_900 |913.88 MHz |
|CH_06_900 |916.04 MHz |
|CH_07_900 |918.20 MHz |
|CH_08_900 |920.36 MHz |
|CH_09_900 |922.52 MHz |
|CH_10_900 |924.68 MHz |
|CH_11_900 |926.84 MHz |
|CH_12_900 |915 MHz |






| Region  | LoRa Frequency Band | LoRa Channel Frequency |
| :------------ | :------------ | :------------ |
|rrrrrrrrrr |rrrrrrrrrr | rrrrrrrrrr | 
|rrrrrrrrrr |rrrrrrrrrr | rrrrrrrrrr | 

Links
- [LoRa Bands](https://www.rfwireless-world.com/Tutorials/LoRa-frequency-bands.html)



