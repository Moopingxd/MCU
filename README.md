# ສາລະບານ

- **ບົດນຳ**.

- **ບົດທີ 0** Blink

- **ບົດທີ 1** Experiment Blink

- **ບົດທີ 2** Switch

- **ບົດທີ 3** RGB

- **ບົດທີ 4** Buzzer

- **Own Project 1** Ambulance

- **ບົດທີ 5** Potentiometer

- **ບົດທີ 6** Relay

- **ບົດທີ 7** Servo

- **ບົດທີ 8** Seven Segment

- **Own Project 2** Elevator

## ບົດນຳ

  ໄມໂຄຣໂປຣເຊສເຊີ ແລະ ໄມໂຄຄອມພີວເຕີ ເປັນອົງປະກອບທີ່ສຳຄັນໃນຄອມພິວເຕີສະໄໝໃໝ່. ລະບົບອັດຕະໂນມັດ ແລະລະບົບຝັງຕົວ. ໄມໂຄຣໂປຣເຊສເຊີ **(microprocessor)** ເຮັດຫນ້າທີ່ເປັນຫນ່ວຍປະມວນຜົນກາງ **(CPU)** ທີ່ປະຕິບັດຄໍາສັ່ງ ແລະ ຄວບຄຸມການເຮັດວຽກຕ່າງໆ. ໄມໂຄຄອມພີວເຕີ **(microcomputer)** ແມ່ນການປະສົມປະສານຂອງ **microprocessor** ກັບຫນ່ວຍຄວາມຈໍາ ແລະ ອຸປະກອນເສີມເພື່ອເຮັດໃຫ້ມັົນປະຕິບັດຫນ້າວຽກສະເພາະໃດຫນຶ່ງປະສິດທິພາບ.

ບົດ​ລາຍ​ງານ​ນີ້​ໄດ້ສຳຫຼວດການ​ທົດ​ລອງ​ທີ່​ສໍາ​ຄັນ​ທີ່​ສະ​ແດງ​ໃຫ້​ເຫັນ​ເຖິງການ​ເຮັດວຽກ​ພື້ນ​ຖານ​ຂອງ **microcontroller** ໄດ້​. ລວມມີການຄວບຄຸມການປ້ອນຂໍ້ມູນ/ການສົ່ງອອກແບບດິຈິຕອນ. ການເຊື່ອມຕໍ່ເຊັນເຊີ ແລະ ການສື່ສານກັບອຸປະກອນຕ່າງໆ. ການທົດລອງເຫຼົ່ານີ້ນໍາສະເໜີການໃຊ້ງານຕົວຈິງທີ່ຊ່ວຍໃຫ້ເຂົ້າໃຈການເຮັດວຽກ ແລະ ການປະຍຸກໃຊ້ຂອງ **microcontrollers** ໃນສະຖານະການຈິງ.

ຫຼັງຈາກຜ່ານການທົດສອບເຫຼົ່ານີ້, ນັກສຶກສາຈະໄດ້ຮັບປະສົບການທາງດ້ານປະຕິບັດຕົວຈິງໃນການເຊື່ອມຕໍ່ໄມໂຄຣຄອນໂທຣອນເລີກັບອຸປະກອນຕ່າງໆ, ການນຳໃຊ້ເຊັນເຊີ ແລະ ການພັດທະນາໂປຣແກຣມ, ເຊິ່ງເປັນພື້ນຖານສຳຄັນໃນການອອກແບບ ແລະ ພັດທະນາລະບົບທີ່ຊັບຊ້ອນຂຶ້ນໃນອະນາຄົດ.

# ບົດທີ 0
### Blink

###ບົດນຳ

- ຈຸດປະສົງ:
  - ຮຽນຮູ້ທີ່ຈະຄວບຄຸມ LED ເປີດແລະປິດໂດຍໃຊ້ Arduino.
  - ເຂົ້າໃຈຫຼັກການການເຮັດວຽກຂອງຄໍາສັ່ງ digitalWrite() ແລະ delay()

### ອູປະກອນ

- Microcontroller (Arduino)
- LED ໃນຕົວ (ຢູ່ pin 13)

### ການເຊື່ອມຕໍ່ວົງຈອນ

- LED: ໃຊ້ໄຟ LED ໃນຕົວຢູ່ pin 13 ຂອງ Arduino.
- ການສະຫນອງພະລັງງານ: Arduino ສະຫນອງພະລັງງານໃຫ້ກັບວົງຈອນທັງຫມົດ.
![image](https://github.com/user-attachments/assets/a658dfe1-1f6b-4c79-87b9-50ce6205b935)
![image](https://github.com/user-attachments/assets/e2995344-7608-4609-8af2-74299b8ec801)

### ໂຄດທີ່ໃຊ້
```
// C++ code

void setup() {

pinMode(LED_BUILTIN, OUTPUT); // PIN 13

}

void loop() {

digitalWrite(LED_BUILTIN, HIGH);

delay(1000); // Wait for 1000 millisecond(s) = 1 second

digitalWrite(LED_BUILTIN, LOW);

delay(1000); // Wait for 1000 millisecond(s) = 1 second

}
```
### ການເຮັດວຽກຂອງວົງຈອນ

- ກຳນົດ PIN:
- Pin 13 ຖືກຕັ້ງເປັນ OUTPUT ເພື່ອຄວບຄຸມການເປີດ ແລະປິດ LED.
- ເປີດ/ປິດ LED:
- ໃຊ້ຄໍາສັ່ງ digitalWrite(13, HIGH) ເພື່ອເປີດໄຟ LED.
- ໃຊ້ຄໍາສັ່ງ digitalWrite(13, LOW) ເພື່ອປິດໄຟ LED.
- ໃຊ້ delay(1000) ເພື່ອລໍຖ້າ 1 ວິນາທີກ່ອນທີ່ຈະເປີດ ຫຼື ປິດ LED./

# ບົດທີ 1

### Experiment Blink

### ບົດນຳ

ການທົດລອງ "Blink" ເປັນການແນະນໍາເບື້ອງຕົ້ນກ່ຽວກັບການຂຽນໂປຣແກຣມ microcontroller. ໂດຍການຄວບຄຸມ output ດິຈິຕອລໂດຍການໃຊ້ LEDs, ການທົດລອງນີ້ເປັນພື້ນຖານສໍາລັບຄວາມເຂົ້າໃຈກ່ຽວກັບການຈັດການ pin GPIO.

### ອູປະກອນ

Microcontroller (Arduino)

LED

Resistor (220Ω)

Jumper wires

Breadboard

### ການເຊື່ອມຕໍ່ວົງຈອນ

LED ແມ່ນເຊື່ອມຕໍ່ກັບ pin output ໂດຍຜ່ານຕົວຕ້ານທານ. ດ້ວຍຂາລົບທີ່ເຊື່ອມຕໍ່ກັບ GND, Microcontroller Arduino ຈະປ່ຽນສະຖານະຂອງ output ເພື່ອເຮັດໃຫ້ໄຟ LED ກະພິບ.
![image](https://github.com/user-attachments/assets/fa74b3a3-9400-416e-baa0-5bcfd41e3fde)
![image](https://github.com/user-attachments/assets/f86bab11-4f5b-4c58-89e9-4d5b54dec076)

### ໂຄດທີ່ໃຊ້
```
// C++ code

void setup() { pinMode(LED_BUILTIN, OUTPUT); // PIN 13

}

void loop() {

digitalWrite(LED_BUILTIN, HIGH);

delay(1000); // Wait for 1000 millisecond(s) = 1 second

digitalWrite(LED_BUILTIN, LOW);

delay(1000); // Wait for 1000 millisecond(s) = 1 second

}

### ການເຮັດວຽກຂອງວົງຈອນ

Arduino ກຳນົກ pin LED ເປັນ output.

ໂປຣແກຣມເຂົ້າໄປໃນ loop ຢ່າງຕໍ່ເນື່ອງ.

ໄຟ LED ຖືກເປີດໂດຍຕັ້ງ pin output ເປັນ HIGH.

Delay 1 ວິນາທີ.

ໄຟ LED ຖືກປິດໂດຍການຕັ້ງ pin output ເປັນ LOW.

Delay 1 ວິນາທີ.

ຂະ​ບວນ​ການ​ນີ້​ແມ່ນເຮັດ​ຊ​້​ໍ​າ​ຢ່າງ​ບໍ່​ມີ​ກໍາ​ນົດ, ເຮັດໃຫ້ເກີດໄຟກະພິບ​.
```
# ບົດທີ 2

### Switch

### ບົດນຳ

ການທົດລອງ "ສະວິດ" ສະແດງໃຫ້ເຫັນເຖິງການໃຊ້ສະວິດເພື່ອຄວບຄຸມຜົນເອົ້າພຸດເຊັ່ນ: LED ໂດຍໃຊ້ microcontroller. ນີ້ແມ່ນແນວຄວາມຄິດທີ່ສໍາຄັນໃນການຂຽນໂປຣແກຣມ ເນື່ອງຈາກວ່າມັນສະແດງໃຫ້ເຫັນວິທີການອ່ານສະຖານະຂອງ input ທາງກາຍະພາບ ແລະ ຕອບສະຫນອງຕາມຄວາມເຫມາະສົມ.

### ອູປະກອນ

- Microcontroller (Arduino)
- Pushbutton (Switch)
- Resistor (220Ω)
- Jumper wires
- Breadboard

### ການເຊື່ອມຕໍ່ວົງຈອນ

- ປຸ່ມກົດແມ່ນເຊື່ອມຕໍ່ກັບ pin 2 (ການປ້ອນຂໍ້ມູນດິຈິຕອນ) ຂອງ Arduino.
- ຂາຫນຶ່ງຂອງປຸ່ມກົດແມ່ນເຊື່ອມຕໍ່ກັບ GND ແລະ ຂາອື່ນແມ່ນເຊື່ອມຕໍ່ກັບ pin 2.
- LED ແມ່ນເຊື່ອມຕໍ່ກັບ pin LED ໃນຕົວ (ຫຼື pin ດິຈິຕອນອື່ນ) ຜ່ານຕົວຕ້ານທານ. ຂາລົບແມ່ນເຊື່ອມຕໍ່ກັບ GND.
![image](https://github.com/user-attachments/assets/0bbd79a3-230c-4410-b47b-54995b421349)
![image](https://github.com/user-attachments/assets/2980044c-b436-47a8-b9ac-3c1134be91e0)

### ໂຄດທີ່ໃຊ້
```
int buttonState = 0

void setup()

{

pinMode(2, INPUT);

pinMode(LED_BUILTIN, OUTPUT);

Serial.begin(9600);

}

void loop()

{

buttonState = digitalRead(2);

if (buttonState == HIGH) {

Serial.println("Button HIGH");

digitalWrite(LED_BUILTIN, HIGH);

} else {

Serial.println("Button LOW");

digitalWrite(LED_BUILTIN, LOW);

}

delay(10);
```
### ການເຮັດວຽກຂອງວົງຈອນ

- Arduino ເລີ່ມຕົ້ນ pin 2 ເປັນ input ສໍາລັບປຸ່ມກົດ ແລະ pin LED ໃນຕົວເປັນ output.
- ໂປຣແກຣມເຂົ້າສູ່ loop ແລະ ຕິດຕາມສະຖານະຂອງປຸ່ມກົດຢ່າງຕໍ່ເນື່ອງ.
- ຖ້າປຸ່ມກົດ (buttonState ແມ່ນສູງ), LED ໃນຕົວຈະເປີດ.
- ຖ້າປຸ່ມບໍ່ໄດ້ກົດ (buttonState ຕໍ່າ), LED ຈະປິດ.
- ຂະບວນການນີ້ເຮັດຊ້ຳຢ່າງຕໍ່ເນື່ອງ, ຕອບສະໜອງຕາມສະຖານະຂອງປຸ່ມກົດ.

# ບົດທີ 3

### RGB

### ບົດນຳ

ໃນບົດນີ້, ພວກເຮົາຈະສຶກສາກ່ຽວກັບການຄວບຄຸມ RGB LED ໂດຍໃຊ້ Arduino. LED RGB ປະກອບດ້ວຍ LED 3 ຕົວ (ສີແດງ, ສີຂຽວ ແລະ ສີຟ້າ) ເຊິ່ງສາມາດປະສົມກັນເພື່ອສ້າງສີທີ່ແຕກຕ່າງກັນໂດຍການປັບຄວາມສະຫວ່າງຂອງແຕ່ລະສີ. ເຊິ່ງບົດນີ້ຈະສະແດງໃຫ້ຮູ້ເຖິງວິທີການຄວບຄຸມ RGB LED ໂດຍໃຊ້ຄໍາສັ່ງຈາກ Serial Input ເພື່ອເປີດ ຫຼື ປິດສີຕ່າງໆ ຫຼື ປະສົມສີເຫຼົ່ານີ້ເພື່ອສະແດງສີທີ່ແຕກຕ່າງ.

### ອູປະກອນ

- Microcontroller (Arduino)
- RGB LED (ประเภท Common Cathode หรือ Common Anode)
- Resistor (220Ω)
- Jumper wires
- Breadboard

### ການເຊື່ອມຕໍ່ວົງຈອນ

RGB LED ມີ 4 pins ຄື: pin ສໍາລັບແຕ່ລະສີ (ສີແດງ, ສີຂຽວ, ສີຟ້າ) ແລະ pin ສໍາລັບດິນ (ສໍາລັບ Common Cathode) ຫຼື VCC (ສໍາລັບ Common Anode), ແຕ່ລະສີແມ່ນເຊື່ອມຕໍ່ກັບ pin ດິຈິຕອລຂອງ Arduino ໂດຍໃຊ້ຕົວຕ້ານທານໃນວົງຈອນນີ້:

- Pin 9: ສີແດງ
- Pin 10: ສີຂຽວ
- Pin 11: ສີຟ້າ
- Cathode ທົ່ວໄປ: ເຊື່ອມຕໍ່ກັບ GND
  ![image](https://github.com/user-attachments/assets/db27b570-d5e5-4a9e-b2d7-acb7f7ac0a3b)
![image](https://github.com/user-attachments/assets/db4c1daf-2df8-4023-9527-2f4df8045e46)


### ໂຄດທີ່ໃຊ້
```
int ledPins\[\] = {11, 10, 9};

void setup() {

Serial.begin(9600);

for (int pin : ledPins){

pinMode(pin, OUTPUT);

}

}

void loop() {

while (Serial.available() > 0) {

String input = Serial.readStringUntil('\\n');

for (int pin : ledPins){

digitalWrite(pin, LOW);

}

delay(10);

if (input == "on" or input == "rgb" or input == "rbg" or input == "grb" or input == "gbr" or input == "brg" or input == "bgr" ) {

for (int pin : ledPins){

digitalWrite(pin, HIGH);

}
}
else if (input == "off") {

for (int pin : ledPins){

digitalWrite(pin, LOW);

}

}

else if (input == "r") {

digitalWrite(ledPins\[0\], HIGH);

}
else if (input == "g") {
digitalWrite(ledPins\[1\], HIGH);
}
else if (input == "b") {
digitalWrite(ledPins\[2\], HIGH);
}
else if (input == "rg" or input == "gr") {
digitalWrite(ledPins\[0\], HIGH);
digitalWrite(ledPins\[1\], HIGH);
}
else if (input == "rb" or input == "br") {
digitalWrite(ledPins\[0\], HIGH);
digitalWrite(ledPins\[2\], HIGH);
}
else if (input == "gb" or input == "bg") {
digitalWrite(ledPins\[1\], HIGH);
digitalWrite(ledPins\[2\], HIGH);
}
else {
allColors();
}
}
}
void allColors(){
//WHITE
for(int pin : ledPins){
digitalWrite(pin, HIGH);
}
delay(100);
for(int pin : ledPins){
digitalWrite(pin, LOW);
}
delay(100);
for(int pin : ledPins){
digitalWrite(pin, HIGH);
delay(100);
digitalWrite(pin, LOW);
delay(100);
}
for(int i = 0; i < 2; i++){
digitalWrite(ledPins\[i\], HIGH);
}
delay(100);
for(int i = 0; i < 2; i++){
digitalWrite(ledPins\[i\], LOW);
}
delay(100);
for(int i = 0; i < 3; i += 2){
digitalWrite(ledPins\[i\], HIGH);\
}
delay(100);
for(int i = 0; i < 3; i += 2){
digitalWrite(ledPins\[i\], LOW);
}
delay(100);
for(int i = 1; i < 3; i++){
digitalWrite(ledPins\[i\], HIGH);
}
delay(100);
for(int i = 1; i < 3; i++){
digitalWrite(ledPins\[i\], LOW);
}
delay(100);}
```
### ການເຮັດວຽກຂອງວົງຈອນ

- Serial Input: ລະບົບລໍຖ້າການປ້ອນຂໍ້ມູນຈາກ Serial ເຊັ່ນ "on", "off" ຫຼື ຄໍາສັ່ງແຕ່ລະສີເຊັ່ນ "r", "g", "b".
- ການຄວບຄຸມ LED: ຂຶ້ນກັບຄໍາສັ່ງປ້ອນຂໍ້ມູນ, ລະບົບຈະເປີດ ຫຼື ປິດ LED ທີ່ສອດຄ້ອງກັນເຊັ່ນ: ເມື່ອຄໍາສັ່ງແມ່ນ "r", LED ສີແດງຈະເປີດ.
- ການປະສົມສີ: ລະບົບສາມາດປະສົມສີໂດຍການເປີດໄຟ LED ຫຼາຍອັນໃນເວລາດຽວກັນ, ຕົວຢ່າງ "rg" ຈະເປີດສີແດງ ແລະ ສີຂຽວ ເຊິ່ງຈະເປັນສີເຫຼືອງ
- ເອັບເຟັກສີທັງໝົດ: ຟັງຊັ່ນ allColors() ໝູນວຽນຜ່ານສີຕ່າງໆເຊັ່ນ: ສີຂາວ, ສີແດງ, ສີຂຽວ, ສີຟ້າ, ແລະ ການປະສົມຂອງສີເຫຼົ່ານີ້ເພື່ອການສະແດງຜົນແບບຄົບວົງຈອນ.

# ບົດທີ 4
### Buzzer###
### ບົດນຳ
ໃນນີ້, ພວກເຮົາຈະໃຊ້ buzzer (ຫຼື ລໍາໂພງ) ເພື່ອສ້າງສຽງທີ່ແຕກຕ່າງກັນໂດຍອີງໃສ່ໂນດດົນຕີ. ພວກເຮົາຈະໃຊ້ຄໍາສັ່ງ tone () ເພື່ອສ້າງສຽງໂດຍອີງໃສ່ຄວາມຖີ່ທີ່ກໍານົດໄວ້.
### ອູປະກອນ
- Microcontroller (Arduino)
- Buzzer
- Jumper wires
- Breadboard (ຖ້າຕ້ອງການ)
### ການເຊື່ອມຕໍ່ວົງຈອນ

- ເຊື່ອມຕໍ່ pin buzzer ກັບ pin 9 ຂອງ Arduino.
- ເຊື່ອມຕໍ່ຂາອື່ນຂອງ buzzer ກັບ GND.
  ![image](https://github.com/user-attachments/assets/8c330756-2b07-4f70-9915-7ef741970a10)

### ໂຄດທີ່ໃຊ້
```
// Notes frequencies (in Hz) for different pitches

# define NOTE_C2 65

# define NOTE_D2 73

# define NOTE_E2 82

# define NOTE_F2 87

# define NOTE_G2 98

# define NOTE_A2 110

# define NOTE_B2 123

# define NOTE_C3 130

# define NOTE_D3 146

# define NOTE_E3 164

# define NOTE_F3 174

# define NOTE_G3 196

# define NOTE_A3 220

# define NOTE_B3 246

# define NOTE_C4 261

# define NOTE_D4 293

# define NOTE_E4 659

# define NOTE_F4 698

# define NOTE_G4 783

# define NOTE_A4 880

# define NOTE_B4 987

// Melody notes and durations

int melody\[\] = {

NOTE_C3, NOTE_F3, NOTE_G3, NOTE_A3,

NOTE_G3, NOTE_F3, NOTE_A3, NOTE_G3,

NOTE_A3, NOTE_B3, NOTE_C4, NOTE_A3,

NOTE_C4, NOTE_B3, NOTE_A3, NOTE_B3,

NOTE_C4, NOTE_B3, NOTE_A3, NOTE_G3,

NOTE_E3, NOTE_D3, NOTE_E3, NOTE_F3,

NOTE_G3, NOTE_E3, NOTE_C3, NOTE_D3,

NOTE_G2, NOTE_C3, NOTE_D3, NOTE_E3,

NOTE_F3, NOTE_G3, NOTE_F3, NOTE_A3,

NOTE_G3, NOTE_F3, NOTE_E3, NOTE_D3,

NOTE_C3, NOTE_D3, NOTE_E3, NOTE_F3,

NOTE_E3, NOTE_E3, NOTE_D3, NOTE_C3,

NOTE_D3, NOTE_E3, NOTE_G3, NOTE_E3,

NOTE_D3, NOTE_C3, NOTE_C4, NOTE_C4,

NOTE_A3, NOTE_G3, NOTE_A3, NOTE_C4,

NOTE_A3, NOTE_A3, NOTE_D4, NOTE_C4,

NOTE_A3, NOTE_G3, NOTE_E3, NOTE_G3,

NOTE_E3, NOTE_D3, NOTE_C3, NOTE_C3,

NOTE_C3, NOTE_C3, NOTE_C3, NOTE_D3,

NOTE_E3, NOTE_D3, NOTE_C3, NOTE_G3,

NOTE_G3, NOTE_G3, NOTE_G3, NOTE_E3,

NOTE_G3, NOTE_A3, NOTE_B3, NOTE_A3,

NOTE_G3, NOTE_E3, NOTE_A3, NOTE_G3,

NOTE_E3, NOTE_D3, NOTE_C3, NOTE_A2,

NOTE_G2, NOTE_A2, NOTE_C3

};

int noteDurations\[\] = {

2, 2, 4, 2,

2, 2, 4, 2,

2, 2, 4, 2,

2, 1, 2, 2,

2, 2, 2, 2,

4, 2, 2, 2,

2, 2, 2, 1,

2, 2, 3, 2,

2, 1, 2, 2,

2, 2, 2, 1,

2, 2, 2, 2,

2, 2, 3, 2,

2, 2, 2, 2,

2, 1, 2, 2,

2, 3, 3, 2,

2, 2, 2, 2,

2, 2, 2, 1,

3, 2, 2, 3,

3, 3, 2, 3,

2, 2, 2, 2,

2, 1, 2, 2,

2, 3, 3, 2,

2, 2, 2, 2,

2, 2, 2, 2,

2, 2, 1,

};

void setup() {

// No setup needed

}

void loop() {

// Play each note in the melody

for (int i = 0; i < 200; i++) {

int noteDuration = 1000 / noteDurations\[i\]; // Note duration in milliseconds

tone(8, melody\[i\], noteDuration); // Play the note on pin 8

delay(noteDuration \* 1.3); // Pause between notes

noTone(8); // Stop the tone

}

delay(2000); // Pause before repeating the melody

}
```
### ການເຮັດວຽກຂອງວົງຈອນ

- ການຫຼິ້ນ Melody: ໃຊ້ຟັງຊັນ tone() ເພື່ອຫຼິ້ນໂນດທີ່ແຕກຕ່າງກັນຜ່ານ buzzer ທີ່ເຊື່ອມຕໍ່ກັບ pin 9 ຂອງ Arduino, ຄວາມຖີ່ຂອງໂນດແມ່ນຖືກກໍານົດຕາມພາລາມິເຕີທີ່ລະບຸ ແລະ ຄວາມຍາວຂອງໂນດແມ່ນຄວບຄຸມໂດຍຜ່ານ array noteDurations\[\].
- ການຢຸດສຽງ: ຟັງຊັນ noTone() ຖືກນໍາໃຊ້ເພື່ອຢຸດສຽງເມື່ອໂນດໄດ້ສໍາເລັດການຫຼິ້ນ ແລະ ຈະມີ(delay()) ເພື່ອໃຫ້ທຸກໆໂນດມີເວລາຢຸດທີ່ເຫມາະສົມ

# ASSIGNMENT

### Ambulance RGB and Buzzer

### ບົດນຳ

ໃຊ້ RGB ແລະ LED ເປັນໄຟ Silent ເມື່ອກົດປຸ່ມ Switch ເຮັດໃຫ້ໄຟຮຸ່ງສະຫຼັບກັນ ແລະ ມີສຽງອອກຈາກ Buzzer ເມື່ອກົດອີກບາດ ຈະສາມາດປິດການໃຊ້ງານ ແລະ ສາມາດກົດ Button ເພື່ອເຮັດສຽງແກ

### ອູປະກອນ

Adruino Uno

Breadboard

Resistor 220 Ohm

RGB

Button Switch

Buzzer

### ການເຊື່ອມຕໍ່ວົງຈອນ

ຕໍ່ຂາ 5V ໃສ່ບອດຂາ + ແລະ GND ໃສ່ - ຕໍ່ສາຍໄຟໃສ່ RGB ຂາສີແດງ ຕໍ່ສາຍໄຟໃສ່ RGB ໃສ່ຂາສີຟ້າ ແລະ ຕໍ່ກັບ Resistor 220 Ohm ຕໍ່ Buzzer ໃສ່ກັບຂາຂອງ Adruino ແລະ GND ຕໍ່ Button 2 ອັນໃສ່່ກັບ Adruino
 ![image](https://github.com/user-attachments/assets/34c26abe-5ca4-465e-b870-6738ec767dd1)
![image](https://github.com/user-attachments/assets/0a2ddc0b-7bfb-44c2-84be-3dfbefaeb126)

### ໂຄດທີ່ໃຊ້
```

const int buttonPin = 4;

const int button2Pin = 2;

const int buzzerPin = 3;

const int hornBuzzerPin = 5;

const int redPin = 9;

const int bluePin = 10;

bool hornOn = false;

bool ambulanceOn = false;

// ຕົວແປສຳລັບການຈັບເວລາ

unsigned long previousLEDMillis = 0;

unsigned long previousToneMillis = 0;

unsigned long previousFreqMillis = 0;

// ກຳນົດຊ່ວງເວລາຕ່າງໆ

const long ledInterval = 500; // ໄລຍະການກະພິບຂອງໄຟ

const long toneInterval = 30; // ໄລຍະການປ່ຽນສຽງ

// ຕົວແປສຳລັບຄວບຄຸມສຽງໄຊເຣັນ

int currentFreq = 500;

const int minFreq = 500;

const int maxFreq = 1000;

const int freqStep = 50;

void setup() {

pinMode(buttonPin, INPUT_PULLUP);

pinMode(button2Pin, INPUT_PULLUP);

pinMode(buzzerPin, OUTPUT);

pinMode(redPin, OUTPUT);

pinMode(bluePin, OUTPUT);

digitalWrite(buzzerPin, LOW);

digitalWrite(redPin, LOW);

digitalWrite(bluePin, LOW);

Serial.begin(9600);

}

void handleButtons() {

static bool lastButtonState = HIGH;

bool currentButtonState = digitalRead(buttonPin);

// ຈັດການປຸ່ມແກ

hornOn = (digitalRead(button2Pin) == LOW);

// ຈັດການປຸ່ມໄຊເຣັນ

if (lastButtonState == HIGH && currentButtonState == LOW) {

ambulanceOn = !ambulanceOn;

delay(50);

}

lastButtonState = currentButtonState;

}

void handleLEDs() {

unsigned long currentMillis = millis();

if (ambulanceOn && (currentMillis - previousLEDMillis >= ledInterval)) {

previousLEDMillis = currentMillis;

static bool isRed = true;

digitalWrite(redPin, isRed ? HIGH : LOW);

digitalWrite(bluePin, isRed ? LOW : HIGH);

isRed = !isRed;

}

if (!ambulanceOn) {

digitalWrite(redPin, LOW);

digitalWrite(bluePin, LOW);

}

}

void handleSiren() {

unsigned long currentMillis = millis();

if (ambulanceOn && (currentMillis - previousToneMillis >= toneInterval)) {

previousToneMillis = currentMillis;

tone(buzzerPin, currentFreq);

// ປັບຄວາມຖີ່ສຽງ

currentFreq += freqStep;

if (currentFreq > maxFreq) {

currentFreq = minFreq;

}

}

if (!ambulanceOn) {

noTone(buzzerPin);

currentFreq = minFreq;

}

}

void handleHorn() {

if (hornOn) {

tone(hornBuzzerPin, 600);

} else {

noTone(hornBuzzerPin);

}

}

void loop() {

handleButtons(); // ອ່ານສະຖານະປຸ່ມກົດ

handleLEDs(); // ຄວບຄຸມໄຟ LED

handleSiren(); // ຄວບຄຸມສຽງໄຊເຣັນ

handleHorn(); // ຄວບຄຸມສຽງແກ

}
```

### ການເຮັດວຽກຂອງວົງກອນ 

ໃຊ້ RGB ແລະ LED ເປັນໄຟ Silent ເມື່ອກົດປຸ່ມ Switch ເຮັດໃຫ້ໄຟຮຸ່ງສະຫຼັບກັນ ແລະ ມີສຽງອອກຈາກ Buzzer ເມື່ອກົດອີກບາດ ຈະສາມາດປິດການໃຊ້ງານ ແລະ ສາມາດກົດ Button ເພື່ອເຮັດສຽງແກ

# ບົດທີ 5

### Potentiometer

### ບົດນຳ

Potentiometer ຫຼື ຕົວປັບແຮງດັນແມ່ນຕົວຕ້ານທານທີ່ສາມາດປັບໄດ້, ສາມາດເຊື່ອມໂຍງກັບຄ່າຕ່າງໆເຊັ່ນ: ການຄວບຄຸມຄວາມສະຫວ່າງຂອງ LED ຫຼື ຄວາມໄວຂອງມໍເຕີ, ຂຶ້ນຢູ່ກັບການປັບຂອງຜູ້ໃຊ້. ການທົດລອງນີ້ຈະແນະນໍາວິທີການອ່ານຈາກອະນາລັອກ ແລະ ວິທີການໃຊ້ງານ ເພື່ອຄວບຄຸມການດໍາເນີນງານໃນແອັບພິເຄຊັ່ນຕ່າງໆ.

### ອູປະກອນ

- Microcontroller (Arduino)
- Potentiometer
- LED
- Resistor (220Ω)
- Jumper wires
- Breadboard

### ການເຊື່ອມຕໍ່ວົງຈອນ

- ເຊື່ອມຕໍ່ potentiometer ກັບ Arduino ດັ່ງຕໍ່ໄປນີ້:
- ຂາ potentiometer ຊ້າຍໄປຫາ 5V ໃນ Arduino.
- ຂາ potentiometer ຂວາໄປຫາ GND.
- pin ກາງ (wiper) ຂອງ potentiometer ແມ່ນເຊື່ອມຕໍ່ກັບ Analog A0 pin ຂອງ Arduino.
- ເຊື່ອມຕໍ່ LED ກັບ pin 11 ໃນ Arduino.
- ຂາຍາວ (Anode pin) ຂອງ LED ໄປກັບ pin 11.
- ຂາສັ້ນ (ຂາ Cathode) ຂອງ LED ໂດຍຜ່ານ 220Ω resistor ຕໍ່ກັບ GND.
  ![image](https://github.com/user-attachments/assets/b7acc954-6820-46cb-8fc6-5879e0fbd86e)


### ໂຄດທີ່ໃຊ້
```
int analogValue = 0;

int ledValue = 0;

void setup() {
Serial.begin(9600);
pinMode(11, OUTPUT);
}
Void loop() {
analogValue = analogRead(A0);
Serial.println(analogValue);
ledValue = map(analogValue, 0, 1023, 0, 255);
Serial.println(ledValue);
analogWrite(11, ledValue);
delay(10);
Serial.print("Potentiometer: ");
Serial.println(map(1023, 0, 1023, 0, 255)); //255
Serial.print("LED: ");
Serial.println(map(255, 0, 255, 0, 1023));//1023
}
```
### ການເຮັດວຽກຂອງວົງຈອນ

- **potentiometer ແມ່ນເຊື່ອມຕໍ່ກັບ pin A0 ຂອງ Arduino ແລະ LED ແມ່ນເຊື່ອມຕໍ່ກັບ pin 11.**
- **ການອ່ານຄ່າຈາກ potentiometer: ຟັງຊັນ analogRead(A0) ອ່ານຄ່າຈາກ potentiometer ເຊິ່ງຈະໄດ້ຮັບຄ່າລະຫວ່າງ 0 ຫາ 1023**
- **ການແປງຄ່າ Potentiometer ຈະຖືກປ່ຽນຈາກຊ່ວງ 0-1023 ເປັນ 0-255 ໂດຍໃຊ້ຟັງຊັນ map().**
- **ການຄວບຄຸມຄວາມສະຫວ່າງຂອງ LED: ຟັງຊັນ analogWrite(11, ledValue) ຈະປັບຄວາມສະຫວ່າງຂອງ LED ໂດຍອີງໃສ່ຄ່າທີ່ປ່ຽນໄດ້.**
- **ຈໍສະແດງຜົນ Serial: ຄ່າ Potentiometer ແລະ ຄວາມສະຫວ່າງ LED ຖືກສະແດງຢູ່ໃນ Serial Monitor.**

# ບົດທີ 6

## Relay 

### ບົດນຳ

ຣີເລ (Relay) ແມ່ນອຸປະກອນທີ່ໃຊ້ເພື່ອຄວບຄຸມວົງຈອນໄຟຟ້າແຮງດັນສູງດ້ວຍສັນຍານຄວບຄຸມແຮງດັນຕໍ່າຈາກ Arduino ເຊິ່ງເຮັດໃຫ້ພວກເຮົາສາມາດເປີດ-ປິດອຸປະກອນໄຟຟ້າພາຍນອກເຊັ່ນ: ດອກໄຟ, ມໍເຕີ, ຫຼື ອຸປະກອນທີ່ໃຊ້ໄຟຟ້າໃນຄົວເຮືອນ.

ໃນບົດນີ້, ພວກເຮົາຈະໃຊ້ relay 5V ເພື່ອຄວບຄຸມການເປີດ-ປິດຂອງ LED ໂດຍໃຊ້ Arduino.

### ອູປະກອນ

- Microcontroller (Arduino)
- Relay Module
- LED
- Resistor (220Ω)
- Jumper wires
- Breadboard

### ການເຊື່ອມຕໍ່ວົງຈອນ
- ເຊື່ອມຕໍ່ Relay ກັບ Arduino.
- IN PIN (ສັນຍານຄວບຄຸມ) ຂອງ Relay → LED_BUILTIN pin (pin 13) ຂອງ Arduino.
- GND pin ຂອງ relay → GND ຂອງ Arduino
- VCC pin ຂອງ relay → 5V ຂອງ Arduino
- ເຊື່ອມຕໍ່ LED ກັບ relay ໄດ້.
- COM (ທົ່ວໄປ) pin ຂອງ relay →ເຊື່ອມຕໍ່ກັບ pole ບວກຂອງ LED ໄດ້.
- NO (ເປີດປົກກະຕິ) pin of relay → ເຊື່ອມຕໍ່ກັບ 5V ຂອງ Arduino.
- ຂົ້ວລົບຂອງ LED → 220Ω resistor → GND ຂອງ Arduino.
  ![image](https://github.com/user-attachments/assets/42d198ea-c9a3-4561-8bea-cf77d8b35f7f)

### ການເຊື່ອມຕໍ່ວົງຈອນ
```
// C++ code

void setup()

{

pinMode(LED_BUILTIN, OUTPUT);

}
void loop()
{
digitalWrite(LED_BUILTIN, HIGH);
delay(1000); // Wait for 1000 millisecond(s)
digitalWrite(LED_BUILTIN, LOW);
delay(1000); // Wait for 1000 millisecond(s)
}
```
### ການເຮັດວຽກຂອງວົງຈອນ

- **Arduino ຄວບຄຸມ relay: ເມື່ອສັນຍານ HIGH ຖືກສົ່ງໄປຫາ LED_BUILTIN (pin 13), relay ຈະປິດວົງຈອນ (ເປີດ LED).**
- **Delay 1 ວິນາທີ: Arduino ຈະລໍຖ້າ 1 ວິນາທີກ່ອນທີ່ຈະປ່ຽນສະຖານະ.**
- **ປ່ຽນສະຖານະ: Arduino ປ່ຽນສັນຍານເປັນ LOW, ເຊິ່ງເຮັດໃຫ້ Relay ເປີດວົງຈອນ (ປິດໄຟ LED).**
- **ເຮັດຊ້ຳ: ລະບົບເປີດ ແລະ ປິດໄຟ LED ທຸກ 1 ວິນາທີ.**

# ບົດທີ 7

### Servo

### ບົດນຳ

ເຕີເຊີໂວ (Servo Motor) ແມ່ນມໍເຕີທີ່ສາມາດ rotate ກັບຕໍາແຫນ່ງທີ່ຊັດເຈນ. ມັນຖືກນໍາໃຊ້ທົ່ວໄປໃນຫຸ່ນຍົນ ຫຼື ລະບົບການຄວບຄຸມອັດຕະໂນມັດ. ບົດນີ້ແມ່ນກ່ຽວກັບວິທີການຄວບຄຸມ servo motor ໂດຍໃຊ້ Potentiometer

### ອູປະກອນ

- Microcontroller (Arduino)
- Servo motor
- Potentiometer
- Jumper wires
- Breadboard

### ການເຊື່ອມຕໍ່ວົງຈອນ

- ເຊື່ອມຕໍ່ຂາ VCC ຂອງ servo ກັບ 5V ໃນ Arduino.
- ເຊື່ອມຕໍ່ GND pin ຂອງ servo ກັບ GND ຂອງ Arduino.
- ເຊື່ອມຕໍ່ສາຍສັນຍານຂອງ servo ກັບ pin 9 ຂອງ Arduino.
- ເຊື່ອມຕໍ່ pin 1 ຂອງ potentiometer ກັບ 5V ໃນ Arduino.
- ເຊື່ອມຕໍ່ pin 2 (ກາງ) ຂອງ Potentiometer ກັບ A0 ຂອງ Arduino.
- ເຊື່ອມຕໍ່ pin 3 ຂອງ Potentiometer ກັບ GND ຂອງ Arduino.
  ![image](https://github.com/user-attachments/assets/bd98ae61-3132-494d-a4ba-65906cc48372)


### ໂຄດທີ່ໃຊ້
```
#include &lt;Servo.h&gt;

Servo myservo; // create servo object to control a servo
int potpin = A0; // analog pin used to connect the potentiometer
int val; // variable to read the value from the analog pin
void setup() {
Serial.begin(9600);
myservo.attach(9); // attaches the servo on pin 9 to the servo object
}
void loop() {
val = analogRead(potpin); // reads the value of the potentiometer (value between 0 and 1023)
Serial.print("pot = ");
Serial.print(val);
Serial.print(", servo = ");
val = map(val, 0, 1023, 0, 180); // scale it to use it with the servo (value between 0 and 180)
Serial.println(val);
myservo.write(val); // sets the servo position according to the scaled value
delay(15); // waits for the servo to get there
}
```
### ການເຮັດວຽກຂອງວົງຈອນ

- **Arduino ອ່ານຄ່າຈາກ potentiometer ທີ່ມີລະດັບ 0-1023.**
- **ໃຊ້ຟັງຊັນ map(val, 0, 1023, 0, 180); ແປງຄ່າເປັນມຸມ 0-180 ອົງສາ.**
- **ໃຊ້ myservo.write(val); ເພື່ອສັ່ງໃຫ້ servo motor ໝຸນໄປກັບມຸມທີ່ຕ້ອງການ**
- **ຄ່າມຸມແມ່ນສະແດງຢູ່ໃນ Serial Monitor.**
- **ໃນເວລາທີ່ໝຸນ potentiometer ເຫັນໄດ້ວ່າ servo motor ໝຸນຕາມມຄ່າທີ່ໄດ້ຮັບ.**

# ບົດທີ 8

### Seven Segment 

### ບົດນຳ

7-Segment Display ເປັນອຸປະກອນສະແດງຜົນທີ່ໃຊ້ກັນຢ່າງກວ້າງຂວາງເຊັ່ນ: ໃນເຄື່ອງຄິດເລກ ຫຼື ໂມງດິຈິຕອນ ເຊິ່ງກ່ຽວກັບການນຳໃຊ້ 7-Segment Display ແບບ1 ຫຼັກດ້ວຍ Arduino ເພື່ອສະແດງຕົວເລກ 0-9.

### ອູປະກອນ

- Microcontroller (Arduino)
- 7-Segment Display LED
- Resistor (220Ω)
- Jumper wires
- Breadboard

### ການເຊື່ອມຕໍ່ວົງຈອນ

ຈໍສະແດງຜົນ 7-Segment ມີ 7 pins (a-g) ເພື່ອສະແດງຕົວເລກ ແລະ common cathode (CC) ຫຼື common anode (CA) pin ເພື່ອກໍານົດປະເພດຂອງການດໍາເນີນງານ.

- ເຊື່ອມຕໍ່ pins a-g ຂອງ 7-Segment ກັບ Arduino pins:

a → 2, b → 3, c → 4, d → 5, e → 6, f → 7, g → 8

- ເຊື່ອມຕໍ່ cathode ທົ່ວໄປ (CC) ຫຼື anode ທົ່ວໄປ (CA) pin ກັບ GND ຫຼື 5V ຕາມປະເພດຂອງ 7-Segment.
- ໃຊ້ຕົວຕ້ານທານ 220Ω ເປັນຊຸດກັບແຕ່ລະ pin a-g ເພື່ອຫຼຸດຜ່ອນກະແສໄຟຟ້າ.
  ![image](https://github.com/user-attachments/assets/77c82aeb-b83f-47b0-ad45-169ae3593271)


### ໂຄດທີ່ໃຊ້
```
// Define the pins for each segment of the display

int segmentPins\[\] = {2, 3, 4, 5, 6, 7, 8}; // Adjust based on your wiring

// Digits representation for common cathode display

byte digits\[\] = {

B11111100, // 0

B01100000, // 1

B11011010, // 2

B11110010, // 3

B01100110, // 4

B10110110, // 5

B10111110, // 6

B11100000, // 7

B11111110, // 8

B11110110 // 9

};

void setup() {

// Set all segment pins as OUTPUT

for (int i = 0; i < 7; i++) {

pinMode(segmentPins\[i\], OUTPUT);

digitalWrite(segmentPins\[i\], LOW); // Turn off all segments initially

}

}

void loop() {

// Display numbers 0 to 9

for (int i = 0; i <= 9; i++) { // Start from 0

displayDigit(i);

delay(1000); // Wait for 1 second

}

// Turn off the display for 1 second

clearDisplay();

delay(1000);

// Display numbers 9 to 0

for (int i = 9; i >= 0; i--) { // Go down to 0

displayDigit(i);

delay(1000); // Wait for 1 second

}

// Turn off the display for 1 second

clearDisplay();

delay(1000);

}

void displayDigit(int num) {

byte segments = digits\[num\];

for (int i = 0; i < 7; i++) {

digitalWrite(segmentPins\[i\], bitRead(segments, 7 - i) ? HIGH : LOW); // Update each segment

}

}

void clearDisplay() {

for (int i = 0; i < 7; i++) {

digitalWrite(segmentPins\[i\], LOW); // Turn off all segments

}

}
```
### ການເຮັດວຽກຂອງວົງຈອນ

- Arduino ສົ່ງສັນຍານໄປຫາ 7-Segment Display ຜ່ານ pins ທີ່ກໍານົດໄວ້.
- ໃຊ້ອາເຣ digits\[\] ເພື່ອກໍານົດລໍາດັບທີ່ LED ແຕ່ລະອັນຈະເປີດແລະປິດເພື່ອສະແດງຕົວເລກທີ່ຖືກຕ້ອງ.
- ໃນວົງ()
- ສະແດງຕົວເລກ 0-9, ແຕ່ລະຕົວເລກໃຊ້ເວລາ 1 ວິນາທີ.
- ປິດໄຟທັງໝົດເປັນເວລາ 1 ວິນາທີ.
- ສະແດງຕົວເລກ 9-0 ໂດຍແຕ່ລະຕົວເລກໃຊ້ເວລາ 1 ວິນາທີ.
- ປິດໄຟທັງໝົດເປັນເວລາ 1 ວິນາທີ.
- ໃຊ້ຟັງຊັນ displayDigit(int num) ເພື່ອສະຫຼັບແຕ່ລະ 7-Segment ເປີດ/ປິດ.
- ໃຊ້ຟັງຊັນ clearDisplay() ເພື່ອລ້າງຈໍສະແດງຜົນ.

# ບົດທີ 10

### Elevator
### ບົດນຳ

ໃຫ້ 7 Segment ສະແດງເລກຊັ້ນທີ່ເຮົາຢູ່ປັດຈຸບັນ ເຮົາສາມາດໃຊ້ Potentiometer ເລືອກຊັ້ນທີ່ຕ້ອງການ 1-2-3 ແລະ ໃຫ້ Servo ໃຊ້ຈຳລອງເປັນມໍເຕີ້ລິບ ເຄື່ອນຕູ້ລິບ ຕາມຊັ້ນເຮົາກົດ Servo ໝຸກໄປກັບ 1 ຮອບ ເທົ່າກັບ 1 ຊັ້ນ

### ອຸປະກອນ

Adruino

Breadboard

Resistor

Potentiometer

7-Segment

Servo

Button

### ການຕໍ່ວົງຈອນ

ຕໍ່ Servo ເຂົ້າກັບ Adruino ຕໍ່ສາຍໄຟ ທີ່ຂາ 5V ໄປໃສ່ຊ່ອງ (+) ແລະ ຕໍ່ GND ໃສ່ (-) ຕໍ່ RGB, Button, Potentiometer, 7- Segment ໃສ່ໃນ Breadboard ຕາມພາບລຸ່ມນີ້
![image](https://github.com/user-attachments/assets/5e39a591-b577-49d2-890b-7971cd400037)

### ການຕໍ່ວົງຈອນ
```
#include &lt;Servo.h&gt;

// Pin Definitions for 7-Segment Display

const int A = 13;

const int B = 12;

const int C = 11;

const int D = 10;

const int E = 9;

const int F = 8;

const int G = 7;

// Other Pin Assignments

const int buttonPin = 2; // Push Button Pin

const int potPin = A0; // Potentiometer Pin

const int servoPin = 6; // Servo Motor Pin

const int doorOpenStatusPin = 3; // LED for Door Open Status

const int doorCloseStatusPin = 4; // LED for Door Close Status

Servo doorServo; // Servo Motor Object

int currentFloor = 1; // Start on Floor 1

int targetFloor = 1; // Target Floor

// Define servo angles corresponding to each floor

const int floorAngles\[\] = {0, 90, 180, 270}; // Angles for floors 1 to 4

void setup() {

Serial.begin(9600); // Initialize Serial Monitor

// Configure 7-Segment Display Pins as Outputs

pinMode(A, OUTPUT);

pinMode(B, OUTPUT);

pinMode(C, OUTPUT);

pinMode(D, OUTPUT);

pinMode(E, OUTPUT);

pinMode(F, OUTPUT);

pinMode(G, OUTPUT);

// Configure Button Pin

pinMode(buttonPin, INPUT_PULLUP);

// Configure Door Status Pins

pinMode(doorOpenStatusPin, OUTPUT); // Door Open LED

pinMode(doorCloseStatusPin, OUTPUT); // Door Close LED

// Attach Servo Motor

doorServo.attach(servoPin);

doorServo.write(floorAngles\[currentFloor - 1\]); // Start at floor 1 position

// Display Initial Floor

displayFloor(currentFloor);

}

void loop() {

// Read Potentiometer Value and Map to Target Floor (1-4)

int potValue = analogRead(potPin);

if (potValue < 256) {

targetFloor = 1;

} else if (potValue < 512) {

targetFloor = 2;

} else if (potValue < 768) {

targetFloor = 3;

} else {

targetFloor = 4; // Adjusted for 4th floor

}

// Print Current and Target Floor to Serial Monitor

Serial.print("Current Floor: ");

Serial.print(currentFloor);

Serial.print(" | Target Floor: ");

Serial.println(targetFloor);

// Wait for Button Press to Confirm Floor Selection

if (digitalRead(buttonPin) == LOW) {

delay(200); // Debounce

Serial.println("Button Pressed. Moving Elevator...");

moveToFloor(targetFloor);

}

// Update 7-Segment Display with the Current Floor

displayFloor(currentFloor);

}

void displayFloor(int floor) {

// Turn Off All Segments

digitalWrite(A, LOW);

digitalWrite(B, LOW);

digitalWrite(C, LOW);

digitalWrite(D, LOW);

digitalWrite(E, LOW);

digitalWrite(F, LOW);

digitalWrite(G, LOW);

// Turn On Segments Based on Floor Number

switch (floor) {

case 1:

digitalWrite(B, HIGH);

digitalWrite(C, HIGH);

break;

case 2:

digitalWrite(A, HIGH);

digitalWrite(B, HIGH);

digitalWrite(D, HIGH);

digitalWrite(E, HIGH);

digitalWrite(G, HIGH);

break;

case 3:

digitalWrite(A, HIGH);

digitalWrite(B, HIGH);

digitalWrite(C, HIGH);

digitalWrite(D, HIGH);

digitalWrite(G, HIGH);

break;

case 4:

digitalWrite(A, HIGH);

digitalWrite(B, HIGH);

digitalWrite(C, HIGH);

digitalWrite(D, HIGH);

digitalWrite(E, HIGH);

digitalWrite(F, HIGH);

break;

}

}

void moveToFloor(int floor) {

if (floor == currentFloor) {

Serial.println("Elevator already on target floor.");

return;

}

Serial.print("Moving from Floor ");

Serial.print(currentFloor);

Serial.print(" to Floor ");

Serial.println(floor);

int step = (floor > currentFloor) ? 1 : -1;

// Simulate movement for each floor using a full 360-degree rotation

while (currentFloor != floor) {

Serial.print("Rotating servo for floor ");

Serial.println(currentFloor + step);

for (int i = 0; i < 360; i++) { // Complete a 360-degree rotation

doorServo.write(i); // Rotate servo

delay(10); // Adjust delay for rotation speed

}

currentFloor += step;

displayFloor(currentFloor);

}

// Open the Door

openDoor();

delay(2000); // Keep Door Open for 2 Seconds

// Close the Door

closeDoor();

}

void openDoor() {

Serial.println("Opening door...");

doorServo.write(180); // Simulate door opening with servo

digitalWrite(doorOpenStatusPin, HIGH); // Turn on LED to indicate the door is open

digitalWrite(doorCloseStatusPin, LOW); // Turn off door close LED

delay(500);

}

void closeDoor() {

Serial.println("Closing door...");

doorServo.write(floorAngles\[currentFloor - 1\]); // Move servo back to floor position

digitalWrite(doorOpenStatusPin, LOW); // Turn off door open LED

digitalWrite(doorCloseStatusPin, HIGH); // Turn on door close LED

delay(500);

}

1. **ການເຮັດວຽກຂອງວົງຈອນ**

ຫຼັງຈາກຕໍ່ວົງຈອນແລ້ວ ເຮົາຈະເຫັນ 7-Segment ສະແດງຊັ້ນທີ່ເຮົາຢູ່ປັດຈຸບັນ ຫຼັງຈາກນັ້ນໃຫ້ເຮົາກົດປຸ່ມເພືອໃຫ້ໄຟເປັນ ສີຟ້າ ແລະ ໝຸນ Potentiometer ເພື່ອເລືອກຊັ້ນໃນ Serial Monitor ແລະ ກົດປຸ່ມເພື່ອຢືນຢັນຊັ້ນທີ່ເລືອກ ຫຼັງຈາກນັ້ນ Servo ຈະ 1 ຮອບ ຕໍ່ 1 ຊັ້ນ
```
# Sheet Lab ການທົດລອງທັງໝົດ
![image](https://github.com/user-attachments/assets/2e601ebe-dd9f-4d08-98c1-26539bb4b897)

[**https://docs.google.com/spreadsheets/d/1fgD1fINyslZyBwaCdMCPx-vJDv68j5T6hoyybIJzzEY/edit?usp=sharing**](https://docs.google.com/spreadsheets/d/1fgD1fINyslZyBwaCdMCPx-vJDv68j5T6hoyybIJzzEY/edit?usp=sharing)
