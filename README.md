# SpineGuard: IoT-Based Real-Time Posture Correction System  
**Tagline**: *"Your Smart Companion for a Healthier Back"*  

## 📌 Overview  
SpineGuard is an IoT-enabled wearable device that monitors spinal posture in real-time using motion sensors, provides corrective feedback, and generates actionable health insights via a cloud-connected dashboard. Designed to combat back pain caused by poor posture, it targets students, office workers, and remote employees.  

### 🌟 **Key Features**  
1. **Real-Time Posture Monitoring**: MPU6050 sensor tracks spine angles.  
2. **Instant Alerts**: Vibration motor/LED triggers on slouching.  
3. **Cloud Dashboard**: Firebase + Supabase for data visualization.  
4. **AI-Powered Insights**: Posture classification and trend prediction (TensorFlow Lite).  
5. **Gamification**: Earn badges for good posture streaks.  
6. **Daily Reports**: Heatmaps, slouch duration, and exercise suggestions.  
7. **Mobile App**: Cross-platform notifications (Flutter).  

---

## 🛠️ Technical Stack  
### **Hardware**  
- **Sensors**: MPU6050 (Accelerometer + Gyroscope), Flex Sensor (Optional).  
- **Microcontroller**: ESP8266 NodeMCU (Wi-Fi) / ESP32 (Advanced).  
- **Actuators**: Vibration Motor, RGB LED.  
- **Power**: 500mAh Li-ion Battery.  

### **Software**  
- **Firmware**: Arduino IDE (C++).  
- **Cloud**: Firebase (Real-Time Alerts), Supabase (User Database).  
- **ML**: TensorFlow Lite (Posture Classification).  
- **Frontend**: React.js (Dashboard), Flutter (Mobile App).  
- **Tools**: PostgresQL, Kalman Filter (Sensor Fusion).  

---

## 📊 Architecture  
```plaintext
                          [SpineGuard Architecture]
                            |
1. Data Acquisition → 2. Edge Processing → 3. Cloud Storage → 4. User Interface  
      (MPU6050)          (ESP8266/ESP32)    (Firebase/Supabase)  (React/Flutter)
```  
1. **Data Acquisition**: MPU6050 captures spine tilt/roll angles at 100Hz.  
2. **Edge Processing**: ESP8266 filters noise (Kalman Filter) and triggers alerts.  
3. **Cloud Storage**:  
   - Firebase: Streams real-time posture status.  
   - Supabase: Stores user profiles, historical data, and exercise recommendations.  
4. **User Interface**: Interactive dashboard with posture heatmaps, streaks, and ML-driven insights.  

---

## 💡 Example Use Cases  
### **User Story 1**: Office Worker  
- **Problem**: Rohan slouches 6+ hours daily while coding.  
- **Solution**: SpineGuard vibrates when he slouches. Weekly report shows a 30% improvement after using app-suggested stretches.  

### **User Story 2**: Student  
- **Problem**: Priya develops neck pain from studying.  
- **Solution**: Heatmap identifies "forward head" posture. ML model recommends ergonomic desk setup.  

---

**Made with ❤️ by [DINESH_AKA_DINESH]**  
