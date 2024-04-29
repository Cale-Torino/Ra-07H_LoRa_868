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