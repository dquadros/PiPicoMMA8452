# Acelerômetro MMA8452Q com Raspberry Pi Pico

Este repositório possui dois módulos MicroPython:

* MMA8452.py: define a classe MMA8452 para interface com o acelerômetro
* demoAcel.py: demonstração usando um display OLED

Componentes para a demonstração:

* Raspberry Pi Pico
* Display OLED 128x64, controlador SSD1306 com interface I2C (endereço padrão, 0x3C) 
* Módulo com acelerômetro MMA8452Q (endereço padrão, 0x1C)

O display e o módulo acelerômetro devem ser alimentados com 3,3V. O sinal SDA dos dois deve ser ligado ao pino GP8 do Raspberry Pi Pico e o sinal SCL ao pino GP9. O pino SA0 do módulo do acelerômetro deve ser ligado a GND. 

Carregar no Pi Pico:

* interpretador MicroPython 
* [driver SSD1306.py](https://github.com/micropython/micropython/blob/master/drivers/display/ssd1306.py)
* MMA8452.py

Na demonstração são apresentadas três barras indicando a aceleração nos três eixos e um quadrado com um ponto para indicar a orientação do sensor.

Mais detalhes no meu blog:
https://dqsoft.blogspot.com
