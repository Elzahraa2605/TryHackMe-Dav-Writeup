# Machine Information

- Machine Name: Dav
- Platform: TryHackMe
- Difficulty: Easy
- Topics Covered: Web Enumeration, WebDAV Exploitation, Privilege Escalation via Sudo misconfigurations.

---

# Lab Overview
المشين دي عبارة عن تحدي (boot2root) يعني الهدف منها إننا نبدأ من الصفر تماماً لحد ما نوصل لأعلى صلاحية في الجهاز وهي الـ (Root). الفكرة الأساسية هنا بتتمحور حولين ثغرات الـ Web Services وتحديداً الـ WebDAV، وازاي الـ Misconfigurations أو الإعدادات الغلط وسوء إدارة الصلاحيات ممكن تفتح باب للمهاجم إنه يسيطر على السيرفر بالكامل.

---

# Initial Enumeration

# Phase 1: Network Scanning

## Execution Parameters
```bash
nmap -sV -Pn 10.128.178.197