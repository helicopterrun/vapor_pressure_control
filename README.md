# Chamber Conditions Control System
Vapor pressure control for an enclosed space for drying/curing and other uses

Pinout:
| PIN | ESP32 I/O | FUNCTION | CODE REQD | Details |
| --- | --------- | -------- | --------- | ------- |
| 1   | GND       | GND      |           |         |
| 2   | GND       | GND      |           |         |
| 3   | IO39/S_VN | Hot fan RPM | pulse counter |         |
| 4   | IO35      | Mirror fan RPM | pulse counter | Input only |
| 5   | IO33      | Output 4 gate | binary output/ledc/slow-pwm |         |
| 6   | IO34      | Cold fan RPM | pulse counter | Input only |
| 7   | IO14      | SPI bus clock | SPI |         |
| 8   | 3.3V OUT  | NC       |           |         |
| 9   | 5V OUT    | NC       |           |         |
| 10  | EN        | NC       |           |         |
| 11  | IO36/S_VP | Circulation fan RPM | pulse counter | Input only |
| 12  | IO26      | Output 1 gate | binary output/ledc/slow-pwm |         |
| 13  | IO18      | Cold fan PWM | LEDC, Fan |         |
| 14  | IO19      | Hot fan PWM | LEDC, Fan |         |
| 15  | IO23      | Circulation fan PWM | LEDC, Fan |         |
| 16  | IO5       | TEC control PWM | LEDC, H-Bridge fan |         |
| 17  | 3.3V OUT  | NC       |           |         |
| 18  | IO13      | SDO/MOSI | SPI     |         |
| 19  | TXT       | NC       |           |         |
| 20  | RXD       | NC       |           |         |
| 21  | IO22      | SCL Bus  | I2C, MUX |         |
| 22  | IO21      | SDA Bus  | I2C, MUX |         |
| 23  | IO17      | Dallas 1-wire | Dallas |         |
| 24  | IO16      | RTD CS Pin | SPI     |         |
| 25  | GND       | GND      |           |         |
| 26  | 5V IN     | 5V Input |           |         |
| 27  | IO15      | TEC control FWD/REV | binary output/ H-Bridge fan |         |
| 28  | GND       | GND      |           |         |
| 29  | IO27      | Output 2 gate | binary output/ledc/slow-pwm |         |
| 30  | IO25      | Mirror fan PWM | LEDC, Fan |         |
| 31  | IO32      | Output 3 Gate | binary output/ledc/slow-pwm |         |
| 32  | IO12      | SDI/MISO | SPI     |         |
| 33  | IO4       | ADC_A/TEC drive current | ADC | ADC2_CH0 |
| 34  | IO0       | NC       |           |         |
| 35  | IO2       | NC       |           |         |
| 36  | NC        | NC       |           |         |
