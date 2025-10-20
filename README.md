# 💌 Love Advisor Bot (n8n Flow Framework)

Framework สำหรับสร้าง Chatbot ที่ปรึกษาความรัก  
สร้างด้วย **n8n + LLM (Google Gemini / OpenAI ฯลฯ)**  
ใช้ **regex** และ **routing logic** เพื่อเลือก prompt ที่เหมาะสม  

> ❗ หมายเหตุ: นี่คือ **Framework** ไม่ใช่บอทสำเร็จรูป  
ผู้ใช้ต้องออกแบบ **Prompt** และ **Closing Messages** เอง

---

## 🎯 Features

- 📩 รองรับ **LINE Messaging API** ผ่าน Webhook
- 🔀 **Routing**: จัดหมวดหมู่ข้อความ เช่น  
  `conflict`, `family`, `sex`, `deeptalk`, `romance`, `breakup`, `trust` ฯลฯ
- 🧠 **Memory**: เก็บ context ระหว่างสนทนาด้วย Buffer Memory
- 🚨 **Safety Flag**:  
  `isCritical=true` สำหรับข้อความเสี่ยง (ฆ่าตัวตาย, ข่มขืน, เพศไม่ยินยอม) → ตัดบทตอบด้วยข้อความปลอดภัย
- 👥 **Dual Persona**:
  - **ศิราณี Mode** → โทนอ่อนโยน อบอุ่น สไตล์ Club Friday  
  - **Buddy Mode** → โทนเพื่อนสนิท ดิบ ๆ แต่ไม่เหยียด

---

## 📦 Installation

1. ติดตั้ง [n8n](https://n8n.io)  
2. Import ไฟล์ `love-consultant.json` ลงใน Workflow

---

## 📖 Usage

1. ผู้ใช้พิมพ์ข้อความเข้า LINE → Webhook รับค่า  
2. Flow สกัดข้อความ → เลือก Route และ Persona ที่เหมาะสม  
3. AI Agent ประมวลผลและสร้างคำตอบ  
4. ระบบส่งข้อความกลับไปที่ LINE

---

## ⚠️ Disclaimer

- Repo นี้แจกเป็น **framework** สำหรับนักพัฒนา/นักวิจัย  
- ผู้ใช้ต้องรับผิดชอบการใช้งานจริง โดยเฉพาะ **คำปรึกษาด้านจิตวิทยา/สุขภาพจิต**  
- ทีมผู้พัฒนา **ไม่รับผิดชอบ** หากมีการนำไปใช้ผิดวัตถุประสงค์

---

## 📝 License

**MIT License**  
- ใช้ได้อิสระเพื่อการเรียนรู้และพัฒนา  
- ⚠️ **Prompt และ Closing Logic ที่ใช้ใน Demo ไม่รวมใน Repo**  
ผู้ใช้ต้องออกแบบเอง
