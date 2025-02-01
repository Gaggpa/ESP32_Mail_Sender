# **ESP32 Gmail Sender**  

## **Overview**  
This project enables the **ESP32** microcontroller to send emails via **Gmail** using WiFi. The ESP32 connects to a WiFi network and sends emails automatically based on predefined conditions or triggers.  

## **Features**  
- Sends emails via **Gmail** from an ESP32.  
- Uses **WiFi** for internet connectivity.  
- Secure authentication using **App Passwords**.  

## **Requirements**  
- **ESP32 Board**  
- **2.4 GHz WiFi** (ESP32 **does not support 5 GHz WiFi**)  
- **Gmail Account** (with an App Password)  

## **Important Considerations**  
1. **WiFi Compatibility:** Ensure that your ESP32 is connected to a **2.4 GHz WiFi network**, as it does **not** support **5 GHz**.  
2. **App Password Required:** Since Google restricts direct password usage, you **must generate an App Password** instead of using your Gmail account password.  

---

## **Generating an App Password in Gmail**  
Follow these steps to create an **App Password** for ESP32:  

### **Step 1: Enable 2-Step Verification**  
1. Go to [Google Account Security](https://myaccount.google.com/security).  
2. Scroll down to **"Signing in to Google"**.  
3. Enable **2-Step Verification** if it's not already enabled.  

### **Step 2: Generate an App Password**  
1. In the **Security** section, go to **"App Passwords"**.  
2. Click **"Select App"** → Choose **"Mail"**.  
3. Click **"Select Device"** → Choose **"Other"**, then type **ESP32**.  
4. Click **"Generate"**, and Google will provide a **16-character** App Password.  
5. **Save this password** or take a **screenshot**, as you won’t be able to view it again.  

---

## **Usage**  
1. Replace your **WiFi credentials** and **Gmail App Password** in the ESP32 code.  
2. Upload the sketch to your ESP32 using **Arduino IDE** or **PlatformIO**.  
3. Monitor the ESP32 serial output for email sending status.  

---

## **Author**  
**Gagpa**  