MFRC522
=======

MFRC522 fork from https://github.com/miguelbalboa/rfid to IDF ESP32

USAGE
=====

```sh
SPI _SPI(VSPI_HOST);
_SPI.init(5); //5==SS
MFRC522 _MFRC522(&_SPI, 22); //22==RST

_MFRC522.PCD_Init();
_MFRC522.PCD_DumpVersionToSerial();
```

EXAMPLE
=======
https://github.com/ericogr/idf-mfrc-card-reader-example
