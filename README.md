# Ra-07H_LoRa_868

N.B

Peer to Peer LoRa with asr6501 is not possible, it is designed for only LoRaWan.

# Steps to send data

1. join

AT+CJOIN=1,0,8,8

2.


Ra-07H

## Settings

COM9

Default: 115200

---

## Join Mode

0 ：OTAA
1：ABP
```
AT+CJOINMODE?
```

## Join

0 ：OTAA
1：ABP
```
AT+CJOIN?

AT+CJOIN=1,0,8,8

//example
ASR6501:~# AT+CJOIN?
+CJOIN:0,0,8,8
OK

```

## Send/Receive

The AT+DTRX command can only be used after joining the LoraWAN network.

See notice at the bottom of the command description.

Notice: It is need to first join into the network, then send data later.

Send/Receive +DTRX

```
AT+DTRX=?

//example
AT+DTRX=1,2,10,0123456789
OK+SEND:03
OK+SENT:01
OK+RECV:02,01,00
```

AT+CTX=868123000,0,22
AT+CRX=868123000,0

## Reboot

0 ：Restart the communication module immediately
1 ：Wait for the wireless frame currently being sent in the

```
AT+IREBOOT=0
```

## Sleep

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
- [P2P not supported](https://forum.m5stack.com/topic/3746/lora-module-asr6501-with-arduino/10)


