# Li-Fi Communication System 🚀  

## 📖 Overview  
This project demonstrates a **Li-Fi communication system** built using **Arduino Uno** and the **LiFiProject application**. The application transmits binary light signals, which are detected, decoded, and displayed in real-time. This innovative project showcases the potential of Li-Fi (Light Fidelity) as a secure and efficient wireless communication technology.  

---

## 💡 Features  
- **Real-Time Communication:** Decodes light signals transmitted via the LiFiProject app.  
- **Predefined Messages:** Displays multiple predefined messages based on transmitted binary patterns.  
- **Seamless Hardware Integration:** Combines Arduino Uno, LiquidCrystal LCD, and LDR for efficient communication.  
- **Interactive Demonstration:** Uses the LiFiProject app for an engaging, hands-on experience.  

---

## 🔧 Components Used  
### Hardware:  
1. **Arduino Uno** (Microcontroller)  
2. **LiquidCrystal LCD (16x2)** (Displays decoded messages)  
3. **Light Dependent Resistor (LDR)** (Detects light signals)  
4. Resistors (1kΩ, 10kΩ for voltage division)  
5. Breadboard and jumper wires  

### Software:  
1. **Arduino IDE** for coding and uploading the sketch.  
2. **LiFiProject Application** for transmitting light signals.  

---

## 🛠️ How It Works  
1. **Signal Transmission:**  
   - The **LiFiProject application** sends binary light signals (ON/OFF patterns).  
   - These patterns represent predefined messages.  

2. **Signal Detection:**  
   - The LDR senses the light signals and converts them into digital inputs for the Arduino.  

3. **Message Decoding:**  
   - Binary patterns are accumulated and matched with predefined sequences:  
     - `001` → "hi"  
     - `0001` → "hello"  
     - `00001` → "how are you?"  
     - ...and more.  

4. **Message Display:**  
   - The decoded message is shown on the **LCD screen** and logged to the **Serial Monitor**.  

---


---

## 🚀 How to Run  
1. **Clone the Repository:**  
   ```bash  
   git clone https://github.com/bhuvan555/LiFi-Communication-System.git  
