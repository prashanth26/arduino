# [Paul McWhorter Tutorial](https://www.youtube.com/playlist?list=PLGs0VKk2DiYw-L-RibttcvK-WBZm8WLEP) Notes

## Arduino Tutorial 1: Setting Up and Programming the Arduino for Absolute Beginners
- Download Arduino IDE from [https://www.arduino.cc/](https://www.arduino.cc/)
- Try a simple light blinking program on port 13

## Arduino Tutorial 2: Understanding How Light Emitting Diodes (LEDs) Work
- LED works as P and N semi conductor
- Only one side
- Long Side (P) - connect to postive
- Short Side (N) - connect to negative

## Arduino Tutorial 3: Understanding How Breadboards Work
- Always use 330 ohm resistance in series with LED of 5V

## Arduino Tutorial 4: Understanding Arduino Variables
- Always use variables instead of literals (strings, numbers)

## Arduino Tutorial 5: Understanding and Working With Binary Numbers
- Anything in the world can be represent as a numbers
- Numbers are then converted into binary

## Arduino Tutorial 6: Build an LED Binary Counter
- All negatives/ground are the same
- Ground can be shared

## Arduino Tutorial 7: Understanding the Arduino Analog Write Command
- You can adjust analog signals from 0-255
- setup() - `pinMode(redPin, OUTPUT)`
- loop() - `analogWrite(redPin, 255)`

## Arduino Tutorial 8: Understanding Pulse Width Modulation (PWM) and the Arduino Analog Write Command
- Pulse modulation
- In Arduino, the analogue modulation for 5V to 2.5V is done using 4 periods alternating between low and high
- If you want pure analogue voltage, you put a capacitor across (in this case 1000microF capacitor)

## Arduino Tutorial 9: Understanding Ohm's Law and Simple Circuit Design
- Circuit analysis
- V = IR
- In series
  - RE = R1 + R2
  - V1 = I * R1
  
## Arduino Tutorial 10: Understanding How To Read Analog Voltage using analogRead Command
- Reading from Analog pin
```
int readPin=A3;
int v2=0;
int delayTime=500;

void setup() {
  pinMode(readPin, INPUT);
  Serial.begin(9600); // Setting serial monitor
}

void loop(){
  v2 = analogRead(readPin);
  Serial.println(v2); // Reads any value between (0-1024)
  delay(delayTime);
}
```
- Reads any value between (0-1024)
- OP: 1023



