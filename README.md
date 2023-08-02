# s2_mini
## Requirimientos
1. esptool
2. firmware a instalar (se puede descargar [aquí](https://github.com/wemos/micropython/releases) )
3. el nombre del puerto serie

## Instalación
1. Presionar botón 0 y dar un pulso en botón reset
2. Ejecutar esptool.py --chip esp32s2 --port /dev/ttyACM0 erase_flash
3. Ejecutar esptool.py --chip esp32s2 --port /dev/ttyACM0 --baud 1000000 write_flash -z 0x1000 firmware-LOLIN_S2_MINI-v1.20.0-124-g17c3f6b6a.bin

### Notas
* */dev/ttyACM0* es el nombre del puerto serie
* *firmware-LOLIN_S2_MINI-v1.20.0-124-g17c3f6b6a.bin* es el nombre del archivo con el firmware 
