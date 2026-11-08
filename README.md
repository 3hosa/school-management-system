# 🏫 School Management System | نظام إدارة المدارس والطلاب

[![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?logo=php&logoColor=white)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?logo=docker&logoColor=white)](https://www.docker.com/)
[![Railway](https://img.shields.io/badge/Railway-Deployable-0B0D0E?logo=railway&logoColor=white)](https://railway.app/)
[![License](https://img.shields.io/badge/License-Proprietary-red.svg)](LICENSE)

---

## 📌 نبذة عامة (Project Overview)

**نظام إدارة المدارس (School Management System)** هو نظام معلوماتي وإداري متكامل مصمم لأتمتة العمليات المدرسية اليومية ومتابعة الحضور والغياب، الدرجات الأكاديمية، شؤون المعلمين، وبيانات الطلاب مع تقارير شاملة.

تم تجهيز النظام ببيئة **Docker** جاهزة للتشغيل السحابي والربط التلقائي بقواعد بيانات MySQL.

---

## 🏗️ الوحدات والوحدات الوظيفية (Core Modules)

```
school-management-system/
├── auth/                 # نظام تسجيل الدخول والتحقق من صلاحيات المعلمين والإداريين
├── students/             # سجلات الطلاب، الملفات الشخصية، وبيانات القيد
├── teachers/             # بيانات الكادر التعليمي، التخصصات، وتوزيع الجداول
├── attendance/           # تسجيل ورصد حضور وغياب الطلاب اليومي والحصص
├── subjects/             # إدارة المواد الدراسية والمناهج وتوزيع الفصول
├── grades/               # رصد درجات الاختبارات، المعدلات، وإصدار الشهادات
├── config/               # إعدادات الاتصال بقاعدة البيانات والبيئة
├── database/             # ملفات الجداول والتهيئة (SQL Schemas)
├── Dockerfile            # حاوية التشغيل وبيئة أباتشي/PHP
└── railway.json          # إعدادات النشر السحابي التلقائي
```

---

## 🌟 الميزات الجوهرية (Key Features)

* **إدارة الطلاب وشؤون القيد:** تسجيل الطلاب، توزيع الفصول الدراسية، وحفظ السجلات الأكاديمية.
* **رصد الحضور والغياب (Attendance Tracking):** تقارير حضور فورية للطلاب مع إحصائيات نسب الحضور والغياب المبرر وغير المبرر.
* **نظام العلامات والتقييم (Grading Engine):** حساب تلقائي للمعدلات والنتائج الفصلية والنهائية.
* **بوابة الكادر التعليمي (Faculty Portal):** لوحة وصول لكل معلم لإدخال درجات فصوله وتسجيل الحضور.

---

## 🚀 دليل التشغيل السريع (Getting Started)

### الخيار 1: باستخدام Docker
```bash
docker build -t school-system .
docker run -d -p 8080:80 --name school_app school-system
```

### الخيار 2: عبر الخادم المحلي (XAMPP / LAMP)
1. استيراد ملفات قاعدة البيانات من مجلد `database/` إلى خادم MySQL.
2. ضبط بيانات الاتصال في ملف `config/database.php` أو `.env`.
3. الدخول عبر المتصفح إلى: `http://localhost/school-management-system`.

---

## 📄 الترخيص (License)
جميع الحقوق محفوظة للمطور © **3hosa**. هذا المشروع خاص وغير مرخص للنشر التجاري أو التعديل دون موافقة مسبقة.
