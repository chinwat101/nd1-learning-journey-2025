# nd1-learning-journey-2025

# IoT Concepts

## MQTT คืออะไร 
โปรโตคอลสื่อสารแบบเบา (lightweight) ออกแบบมาสำหรับ IoT และอุปกรณ์ทรัพยากรจำกัด ใช้แบนด์วิดท์ต่ำ หน่วงต่ำ และทนเครือข่ายไม่เสถียร


# MQTT Connection Taxonomy

## 1. Core Architecture
### 1.1 Publish / Subscribe Model
- Publisher: ส่งข้อมูลไปยัง Topic
- Subscriber: รับข้อมูลจาก Topic
- Broker: ตัวกลางจัดการการรับ–ส่งข้อความ

### 1.2 Client Types
- Sensor Node (ESP32, MCU)
- Gateway / Edge Device
- Backend Server
- Web / Mobile Application

---

## 2. Network Connection Types
### 2.1 Transport Layer
- TCP/IP (มาตรฐาน)
- TCP/IP + TLS (Secure MQTT)
- WebSocket (MQTT over WS)

### 2.2 Network Environment
- Local Network (LAN)
- Internet / Cloud
- Cellular Network (4G / 5G / NB-IoT)
- Low-bandwidth / Unstable Network

---

## 3. Broker Deployment Models
### 3.1 Local Broker
- On-device
- On-premise Server

### 3.2 Cloud Broker
- Public Cloud MQTT
- Private Cloud MQTT

### 3.3 Clustered Broker
- High Availability
- Load Balancing
- Distributed System

---

## 4. Message Delivery Assurance
### 4.1 Quality of Service (QoS)
- QoS 0: At most once
- QoS 1: At least once
- QoS 2: Exactly once

### 4.2 Message Persistence
- Retained Message
- Persistent Session
- Clean Session

---

## 5. Topic Organization
### 5.1 Hierarchical Topic Structure
- device/{device_id}/status
- location/{area}/sensor/{type}

### 5.2 Topic Filtering
- Single-level wildcard (+)
- Multi-level wildcard (#)

---

## 6. Session Management
### 6.1 Connection State
- Clean Session
- Persistent Session

### 6.2 Keep Alive
- Heartbeat Mechanism
- Timeout Detection

### 6.3 Last Will and Testament (LWT)
- Client Offline Notification
- Failure Detection

---

## 7. Security & Authentication
### 7.1 Authentication
- Username / Password
- Token-based Authentication
- Certificate-based Authentication

### 7.2 Encryption
- TLS/SSL
- Encrypted Payload

### 7.3 Authorization
- Topic-based Access Control
- Read / Write Permission

---

## 8. Integration Patterns
### 8.1 Device to Device
- Sensor → Actuator

### 8.2 Device to Cloud
- IoT Node → Backend

### 8.3 Edge to Cloud
- Edge Gateway → Cloud Analytics

### 8.4 Cloud to Application
- Backend → Dashboard / API

---

## 9. Reliability & Scalability
### 9.1 Fault Tolerance
- Auto Reconnect
- Message Retry

### 9.2 Scalability
- Horizontal Scaling
- Broker Clustering

---

## 10. Typical IoT Use Cases
- Smart Farm
- Smart Home
- Industrial Monitoring
- Real-time Dashboard
