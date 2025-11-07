# n8n-xiao-world

> **n8n Integration for xiao-world** - เชื่อมต่อ n8n กับ xiao-world เพื่อเผยแพร่เนื้อหาจากเสี้ยวหงชูไปยัง Twitter, Facebook, TikTok, YouTube อัตโนมัติ

[![n8n](https://img.shields.io/badge/n8n-Workflow_Automation-blue?style=flat-square)](https://n8n.io)
[![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=flat-square&logo=docker)](https://www.docker.com/)
[![xiao-world](https://img.shields.io/badge/xiao--world-MCP_Server-green?style=flat-square)](https://github.com/huge8888/xiao-world)

---

## 🚀 Quick Start

```bash
# 1. Clone repository
git clone https://github.com/huge8888/n8n-xiao-world.git
cd n8n-xiao-world

# 2. รัน n8n ด้วย Docker Compose
docker-compose up -d

# 3. เปิด n8n
open http://localhost:5678

# 4. Import workflow
# Import workflows/xiao-world-workflow.json
```

**📖 อ่านเอกสารเพิ่มเติม:**
- **[SETUP.md](./SETUP.md)** - คู่มือติดตั้งแบบสั้น (สำหรับคนรู้จัก n8n)
- **[GUIDE.md](./GUIDE.md)** - คู่มือละเอียดทุกขั้นตอน (สำหรับมือใหม่)

---

## 📋 สิ่งที่ต้องมี

ก่อนเริ่มต้อง:
- ✅ Docker & Docker Compose ([ดาวน์โหลด](https://www.docker.com/get-started))
- ✅ **xiao-world รันอยู่แล้ว** ([ติดตั้ง xiao-world](https://github.com/huge8888/xiao-world))
- ✅ API Keys สำหรับ platforms (Twitter, Facebook, etc.)

---

## 📦 ไฟล์ในโปรเจค

```
n8n-xiao-world/
├── README.md                    # เอกสารนี้ (Overview)
├── SETUP.md                     # คู่มือติดตั้งแบบสั้น
├── GUIDE.md                     # คู่มือละเอียดสำหรับมือใหม่
├── docker-compose.yml           # Docker setup สำหรับ n8n
├── workflows/
│   └── xiao-world-workflow.json # Workflow พร้อมใช้งาน (8 nodes)
└── images/                      # Screenshots
```

---

## ✨ Features

### 🔄 Workflow พร้อมใช้งาน
- **8 nodes** ที่เชื่อมต่อกันแล้ว
- **รองรับ multi-platform:** Twitter, Facebook (เพิ่ม TikTok, YouTube ได้)
- **ใช้เวลา ~8-10 วินาที** ต่อการเผยแพร่

### 🐳 Docker Ready
- รัน n8n ด้วยคำสั่งเดียว: `docker-compose up -d`
- เชื่อมต่อ xiao-world อัตโนมัติ
- Data persistence (workflows + credentials)

### 🎯 No-Code Solution
- ไม่ต้องเขียนโค้ด
- ลากวาง node ในแบบ visual
- ปรับแต่งได้ตามต้องการ

---

## 🎮 Workflow ที่เตรียมไว้ให้

### 1. xiao-world-workflow.json (Multi-Platform Publisher)

**8 Nodes:**
1. 🟢 Manual Trigger - เริ่มต้น
2. 📝 Set Feed ID - ตั้งค่า feed_id และ xsec_token
3. 📥 Get Feed Detail - ดึงข้อมูลจากเสี้ยวหงชู (MCP API)
4. 🔧 Parse Data - แปลงข้อมูล
5. 🐦 Publish to Twitter - โพสต์ไป Twitter
6. 📘 Publish to Facebook - โพสต์ไป Facebook
7. 📊 Merge Results - รวมผลลัพธ์
8. ✅ Format Output - แสดงสรุป

**การใช้งาน:**
```bash
# 1. Import workflow
# 2. แก้ไข "Set Feed ID" node ใส่ feed_id และ xsec_token
# 3. Execute!
```

---

## 📚 เอกสาร

| ไฟล์ | คำอธิบาย | เหมาะกับใคร |
|------|----------|-------------|
| **[SETUP.md](./SETUP.md)** | คู่มือติดตั้งแบบสั้น<br/>Prerequisites, Quick Setup, Usage | ผู้ใช้ที่รู้จัก n8n แล้ว |
| **[GUIDE.md](./GUIDE.md)** | คู่มือละเอียดทุกขั้นตอน<br/>มีภาพประกอบ, อธิบายแต่ละ step | มือใหม่ที่ไม่เคยใช้ n8n |

---

## 🔗 Links

- **[xiao-world](https://github.com/huge8888/xiao-world)** - MCP Server หลัก (ต้องติดตั้งก่อน!)
- **[n8n Documentation](https://docs.n8n.io)** - เอกสาร n8n อย่างเป็นทางการ
- **[MCP Protocol](https://modelcontextprotocol.io)** - Model Context Protocol

---

## 🤝 Contributing

ยินดีรับ Pull Requests! ถ้ามี:
- Workflow ใหม่ๆ
- แก้ไข bugs
- ปรับปรุงเอกสาร

---

## 📄 License

MIT License - ใช้งานได้อย่างอิสระ

---

## 🌟 Support

ถ้าชอบโปรเจคนี้ อย่าลืม:
- ⭐ ให้ดาว [xiao-world](https://github.com/huge8888/xiao-world)
- ⭐ ให้ดาว [n8n-xiao-world](https://github.com/huge8888/n8n-xiao-world)

---

<div align="center">

**สนุกกับการทำงานอัตโนมัติ! 🤖✨**

Made with ❤️ for Thai Community 🇹🇭

</div>
