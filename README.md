# LiFi-Communication-System
# Li-Fi Communication System 🚀  

## 📖 Overview  
This project showcases a **Li-Fi communication system** built using **Arduino Uno**. Li-Fi (Light Fidelity) is an innovative wireless communication technology that uses visible light instead of radio waves to transmit data.  
We designed a prototype that can detect light signals, decode them into predefined messages, and display them in real-time on an LCD screen and Serial Monitor. This project highlights the potential of Li-Fi in revolutionizing wireless communication with secure and efficient data transmission.  

---  

## 💡 Features  
- **Real-Time Communication:** Decodes messages transmitted through light signals.  
- **Predefined Messages:** Supports multiple predefined messages based on binary light signals.  
- **Hardware Integration:** Combines Arduino Uno, LiquidCrystal LCD, and LDR for seamless functionality.  
- **Compact Design:** Demonstrates the feasibility of Li-Fi communication in small-scale applications.  

---  

## 🔧 Components Used  
### Hardware:  
1. **Arduino Uno** (Microcontroller)  
2. **LiquidCrystal LCD (16x2)** (Display messages)  
3. **Light Dependent Resistor (LDR)** (Detects light signals)  
4. **Resistors** (1kΩ, 10kΩ for voltage division)  
5. **Jumper Wires**  
6. **Breadboard**  

### Software:  
1. **Arduino IDE** for writing and uploading the code.  

---  

## 🛠️ How It Works  
1. **Light Signal Transmission:**  
   - A light source (e.g., an LED) is used to transmit binary signals (ON/OFF patterns).  
   - The binary patterns represent predefined messages.  

2. **Signal Detection:**  
   - An LDR detects the light signals and converts them into digital signals using the Arduino's `digitalRead` function.  

3. **Message Decoding:**  
   - The system reads the binary sequence and matches it with predefined patterns (e.g., `001 → hi`, `0001 → hello`).  
   - The corresponding message is displayed on the LCD and printed on the Serial Monitor.  

4. **Reset:**  
   - The system resets the binary sequence and waits for the next signal once the message is decoded.  

---  

## 🔍 Code Explanation  
- The `LiquidCrystal` library is used to control the 16x2 LCD.  
- The LDR is connected to pin `8` with `INPUT_PULLUP` mode for detecting light signals.  
- A `String` variable (`duration`) accumulates the binary input and checks for matching patterns.  
- Decoded messages are displayed on the LCD using the `lcd.print()` function and logged to the Serial Monitor.  

---  

## 🚀 How to Run the Project  
1. **Clone the Repository:**  
   ```bash  
   git clone https://github.com/bhuvan555/LiFi-Communication-System.git  
