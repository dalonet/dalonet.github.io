---
layout: post
title: Daftar Port Game Populer untuk Konfigurasi Jaringan
date: 2026-01-10
category: Network
author: Dalonet
thumbnail: "assets/imgs/blog/daftar-port-game-populer.jpg"
excerpt: "Daftar lengkap port TCP/UDP untuk game populer yang berguna untuk konfigurasi firewall, router, atau QoS jaringan."
---

## 📊 Panduan Lengkap Port Game Populer

Port jaringan sangat penting untuk pengalaman bermain game yang optimal. Berikut adalah daftar port yang digunakan oleh game-game populer untuk konfigurasi firewall, QoS (Quality of Service), atau prioritas bandwidth.

### ⚡ Mobile Legends: Bang Bang
**Diperbarui:** 28 Mei 2025

| Mode | Port TCP | Port UDP |
|------|----------|----------|
| All Modes | 30071, 30021, 30102, 5064, 5505, 5562, 5564, 5565, 5568, 5571, 7002, 7003, 7004, 7591 | 30190, 19000, 5015, 5512, 5514, 5515, 5518, 5555, 5521, 6789 |

**Tips:**
- Port 30071-30102 untuk matchmaking utama
- Prioritaskan UDP port untuk ping yang lebih stabil

---

### ♟️ Magic Chess Go Go
**Diperbarui:** 29 Mei 2025

| Mode | Port TCP | Port UDP |
|------|----------|----------|
| Rank | 13701, 14503, 14513, 14515, 14524 | - |

**Catatan:** Game ini hanya menggunakan koneksi TCP untuk komunikasi real-time.

---

### 🔫 Free Fire (FF)
**Diperbarui:** 25 Mei 2025

| Mode | Port TCP | Port UDP |
|------|----------|----------|
| All Modes | 39699, 39801, 6006, 8001, 8012, 7006, 6674 | 10015, 10016, 10018, 6008, 7008 |

**Rekomendasi:**
- Buka port 10015-10018 untuk suara (voice chat)
- Port 39699-39801 untuk server matchmaking

---

### 🎯 PUBG Mobile
**Diperbarui:** 20 Mei 2025

| Mode | Port TCP | Port UDP |
|------|----------|----------|
| All Modes | Dalam pengembangan | Dalam pengembangan |

**Status:** Port untuk PUBG Mobile sedang dalam penelitian dan akan diperbarui segera.

---

## 🛠️ Cara Menggunakan Daftar Port Ini

### 1. **Untuk Router/Modem:**
1. Buka halaman admin router (biasanya 192.168.1.1)
2. Masuk ke menu **Firewall** atau **Port Forwarding**
3. Tambahkan rule baru dengan port dari tabel di atas
4. Set protocol ke **TCP/UDP** atau sesuai kebutuhan

### 2. **Untuk QoS (Quality of Service):**
1. Prioritaskan port game di pengaturan QoS router
2. Atur bandwidth minimum untuk port-port tersebut
3. Simpan konfigurasi dan restart router jika perlu

### 3. **Untuk Firewall Windows:**
```powershell
# Contoh membuka port di Windows Firewall
New-NetFirewallRule -DisplayName "Mobile Legends Ports" -Direction Inbound -Protocol TCP -LocalPort 30071,30021,30102 -Action Allow


