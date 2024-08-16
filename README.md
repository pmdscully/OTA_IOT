# OTA_IOT
Over the air (OTA) binary patching for IOT devices.


Update the firmware using Arduino_ESP_OTA library, following their steps:

> Steps:
> 1. Create a sketch for your ESP board and verify that it both compiles and works.
> 2. In the IDE select: Sketch -> Export compiled Binary.
> 3. Create an OTA update file utilising the tools 'lzss.py' and 'bin2ota.py' stored in https://github.com/arduino-libraries/ArduinoIoTCloud/tree/master/extras/tools .
>     - A. ./lzss.py --encode SKETCH.bin SKETCH.lzss
>     - B. ./bin2ota.py ESP SKETCH.lzss SKETCH.ota
> 4. Upload the OTA file to a network reachable location, e.g. LOLIN_32_Blink.ino.ota has been uploaded to: http://downloads.arduino.cc/ota/LOLIN_32_Blink.ino.ota
> 5. Verify if a custom ca_cert is needed by default DigiCert root CA are used https://www.digicert.com/kb/digicert-root-certificates.htm
> 6. Perform an OTA update via steps outlined below.
>
> Source: https://github.com/arduino-libraries/Arduino_ESP32_OTA/blob/main/examples/OTA_GitHub_Server/OTA_GitHub_Server.ino

