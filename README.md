<div align="center">

# 🔎 TH Health Lens

### ระบบตอบกลับอัตโนมัติในการตรวจสอบข่าวสุขภาพภาษาไทย
**Development of an Automated Health News Verification Response System in Thai**  
*Using Large Language Models and Retrieval-Augmented Generation*

<br/>

[![Web App](https://img.shields.io/badge/🚀%20Web%20Application-Live-success?style=for-the-badge)](http://20.41.105.1:5007/)
[![Project Page](https://img.shields.io/badge/🌐%20Project%20Page-GitHub%20Pages-blue?style=for-the-badge)](https://thamons.github.io/THhealthNewsVerifyPage/)
[![GitHub Repo](https://img.shields.io/badge/📁%20Source%20Code-GitHub-black?style=for-the-badge&logo=github)](https://github.com/thamonS/THhealthNewsVerifyPage)

<br/>

![Accuracy](https://img.shields.io/badge/Accuracy-93%25-brightgreen?style=flat-square)
![F1-Score](https://img.shields.io/badge/F1--Score-0.9027-4CAF50?style=flat-square)
![Dataset](https://img.shields.io/badge/Thai%20Health%20News-3%2C373%20articles-FF9800?style=flat-square)
![Model](https://img.shields.io/badge/Model-Typhoon2--Qwen2.5--7B-9C27B0?style=flat-square)
![Tech](https://img.shields.io/badge/RAG-Retrieval--Augmented%20Generation-2196F3?style=flat-square)
![Year](https://img.shields.io/badge/Senior%20Project-2025-lightgrey?style=flat-square)

</div>

---

## 🌐 ลิงก์สำคัญ / Quick Links

| | ชื่อ | ลิงก์ | คำอธิบาย |
|:---:|:---|:---|:---|
| 🚀 | **Web Application** | [http://20.41.105.1:5007/](http://20.41.105.1:5007/) | ระบบตรวจสอบข่าวสุขภาพ (Live) |
| 🌐 | **Project Page** | [thamons.github.io/THhealthNewsVerifyPage](https://thamons.github.io/THhealthNewsVerifyPage/) | หน้าเว็บโปรเจคหลัก |
| 📁 | **Source Code** | [GitHub Repository](https://github.com/thamonS/THhealthNewsVerifyPage) | โค้ดทั้งหมดของโปรเจค |
| 📄 | **Research Proposal** | [PDF Document](https://thamons.github.io/THhealthNewsVerifyPage/images/%E0%B9%81%E0%B8%81%E0%B9%89_%E0%B9%80%E0%B8%99%E0%B8%B7%E0%B9%89%E0%B8%AD%E0%B8%AB%E0%B8%B2%20form1.pdf) | เค้าโครงงานวิจัย |

---

## 📄 บทคัดย่อ / Abstract

<details open>
<summary><b>🇹🇭 ภาษาไทย</b></summary>

<br/>

> ปัญหาการแพร่กระจายของข่าวปลอมในสื่อออนไลน์เป็นภัยคุกคามสำคัญต่อสังคมไทย โดยข้อมูลจากศูนย์ต่อต้านข่าวปลอมประเทศไทยพบว่า **ข่าวปลอมในหมวดสุขภาพคิดเป็นร้อยละ 36.71** ของทุกหมวด ซึ่งส่งผลกระทบต่อการตัดสินใจด้านสุขภาพของประชาชน
>
> งานวิจัยนี้พัฒนาระบบตอบกลับอัตโนมัติในการตรวจสอบข่าวสุขภาพภาษาไทย โดยใช้แบบจำลองภาษาขนาดใหญ่ร่วมกับเทคนิคการสร้างคำตอบด้วยการดึงข้อมูลภายนอก **(RAG)** จากแหล่งอ้างอิงที่น่าเชื่อถือ เพื่อให้ข้อมูลเป็นปัจจุบันและลดปัญหา Hallucination โดยใช้ข้อมูลข่าวสุขภาพภาษาไทยจำนวน **3,373 ข่าว** จากศูนย์ต่อต้านข่าวปลอมประเทศไทย และใช้โมเดล **Typhoon2-Qwen2.5-7B-Instruct** ทดสอบด้วยชุดข้อมูล 200 ข่าว

**คำสำคัญ:** เทคนิคการสร้างคำตอบจากการดึงข้อมูล · แบบจำลองภาษาขนาดใหญ่ · การประมวลผลภาษาธรรมชาติ · ข่าวปลอมด้านสุขภาพ · ระบบตรวจสอบข่าวสุขภาพภาษาไทย

</details>

<details>
<summary><b>🇬🇧 English</b></summary>

<br/>

> The spread of fake news on social media poses a significant threat to Thai society. The Anti-Fake News Center Thailand reported that **health-related fake news accounted for 36.71% of all categories**, directly impacting public health decision-making.
>
> This research developed an automated Thai health news verification system using Large Language Models (LLMs) combined with **Retrieval-Augmented Generation (RAG)** to retrieve up-to-date information from credible sources, reducing hallucination. The study utilized **3,373 Thai health news articles** and the **Typhoon2-Qwen2.5-7B-Instruct** model, evaluated on a test set of 200 news topics.

**Keywords:** Retrieval-Augmented Generation (RAG) · Large Language Models (LLMs) · Natural Language Processing (NLP) · Health misinformation · Thai health news verification system

</details>

---

## 📊 ผลการทดสอบประสิทธิภาพ / Performance Results

<div align="center">

| ชุดทดสอบ | Accuracy | F1-Score | สถานะ |
|:---|:---:|:---:|:---:|
| **Main Test Set** (ชุดทดสอบหลัก) | **93.00%** | **0.9027** | 🟢 ดีเยี่ยม |
| **Ambiguous Text** (ข้อความคลุมเครือ) | 92.16% | 0.8947 | 🟢 ดีมาก |
| **Misspelled Text** (ข้อความเขียนผิด) | 89.83% | 0.8500 | 🟡 ดี |
| **Negated Text** (ข้อความความหมายตรงข้าม) | 74.36% | 0.7826 | 🟠 พอใช้ |

</div>

---

## ✨ คุณสมบัติของระบบ / Features

- ✅ **ตรวจสอบข่าวสุขภาพภาษาไทย** แบบอัตโนมัติด้วย LLM + RAG
- 📝 **อธิบายเหตุผล** ประกอบการจำแนกประเภทข่าวทุกครั้ง
- 🔗 **แสดงแหล่งอ้างอิง (URLs)** จากแหล่งข้อมูลที่น่าเชื่อถือ
- 💡 **ให้คำแนะนำเพิ่มเติม** ที่เหมาะสมแก่ผู้ใช้งาน
- 🔄 **ข้อมูลเป็นปัจจุบัน** ลด Hallucination ด้วยเทคนิค RAG
- 🇹🇭 **รองรับภาษาไทย** อย่างเต็มรูปแบบ

---

## 🛠️ เทคโนโลยีที่ใช้ / Technology Stack

```
LLM Model  :  Typhoon2-Qwen2.5-7B-Instruct
Technique  :  Retrieval-Augmented Generation (RAG)
Dataset    :  3,373 Thai Health News (Anti-Fake News Center Thailand)
NLP        :  Thai Natural Language Processing
Test Set   :  200 news articles
```

---

## ⚙️ ขั้นตอนการทำงาน / Workflow

### 1️⃣ Data Preparation

![Data Preparation Workflow](https://thamons.github.io/THhealthNewsVerifyPage/images/workflow%20prepare.png)

> การเตรียมข้อมูลข่าวสุขภาพภาษาไทยจาก Anti-Fake News Center Thailand เพื่อสร้างฐานข้อมูลของระบบ RAG

### 2️⃣ System Workflow

![System Workflow](https://thamons.github.io/THhealthNewsVerifyPage/images/workflow%20system.png)

> การทำงานของระบบตั้งแต่รับ input ข่าวจากผู้ใช้ → ค้นหาข้อมูลจากฐานความรู้ → สร้างคำตอบพร้อมแหล่งอ้างอิง

---

## 🚀 Web Application

> 🎯 **ทดลองใช้งานระบบตรวจสอบข่าวสุขภาพจริงได้เลย!**

<div align="center">

### 👉 [คลิกที่นี่เพื่อใช้งาน → http://20.41.105.1:5007/](http://20.41.105.1:5007/)

</div>

---

## 👥 ทีมวิจัย / Research Team

<div align="center">

| | ชื่อ | บทบาท | GitHub |
|:---:|:---|:---:|:---:|
| <img src="https://thamons.github.io/THhealthNewsVerifyPage/images/pornwalai_pic.jpg" width="64" style="border-radius:50%"/> | **พรวลัย ฟ็อกซ์ออล**<br/>Pornwalai Foxall | ผู้วิจัย | [![GitHub](https://img.shields.io/badge/-Pornwalaifoxall-black?logo=github&style=flat-square)](https://github.com/Pornwalaifoxall) |
| <img src="https://thamons.github.io/THhealthNewsVerifyPage/images/thamon_pic.jpg" width="64" style="border-radius:50%"/> | **ธมน ศิริพราหมณกุล**<br/>Thamon Siriprahmanakul | ผู้วิจัย | [![GitHub](https://img.shields.io/badge/-thamonS-black?logo=github&style=flat-square)](https://github.com/thamonS) |
| <img src="https://thamons.github.io/THhealthNewsVerifyPage/images/AjYa.jpg" width="64" style="border-radius:50%"/> | **พิชญา วิรัชโชติเสถียร**<br/>Pitchaya Wiratchotisatian | อาจารย์ที่ปรึกษา | — |

</div>

---

## 📑 เอกสารงานวิจัย / Research Documents

| ไอคอน | เอกสาร | คำอธิบาย | ดาวน์โหลด |
|:---:|:---|:---|:---:|
| 📄 | **เค้าโครงงานวิจัย (Proposal)** | ความเป็นมา · วัตถุประสงค์ · ขอบเขตการวิจัย · เอกสารที่เกี่ยวข้อง · วิธีดำเนินการวิจัย | [📥 PDF](https://thamons.github.io/THhealthNewsVerifyPage/images/%E0%B9%81%E0%B8%81%E0%B9%89_%E0%B9%80%E0%B8%99%E0%B8%B7%E0%B9%89%E0%B8%AD%E0%B8%AB%E0%B8%B2%20form1.pdf) |

---

<div align="center">

🎓 **สาขาวิชาสถิติ เอกสารสนเทศสถิติและวิทยาการข้อมูล**  
Department of Statistics, Information Statistics and Data Science  
**มหาวิทยาลัยขอนแก่น / Khon Kaen University · 2025**

---

*Made with ❤️ by TH Health Lens Research Team*

</div>
