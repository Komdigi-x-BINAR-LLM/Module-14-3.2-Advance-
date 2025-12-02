# Hands-on Komdigi: Modul 3.2 - LLM Guardrails & PII Protection 🛡️

Selamat datang di *repository hands-on* untuk **Modul 3.2 (Advance): Keamanan AI**.

**Tujuan:**
Di modul ini, kita tidak fokus membuat model menjadi "pintar", tapi membuatnya "aman". Notebook ini (`Modul_3_2_Guardrails.ipynb`) akan melatih Anda menggunakan *tools* standar industri untuk membersihkan data sensitif dan memfilter konten berbahaya.

**Materi Praktik:**
1.  **PII Redaction (3.2.4):** Menggunakan **Microsoft Presidio** untuk mendeteksi dan menyensor NIK, No HP, dan Email secara otomatis sebelum data dikirim ke LLM.
2.  **Input Guardrail (3.2.3):** Membuat filter sederhana berbasis *keyword* dan logika untuk mencegah topik terlarang.
3.  **HITL Simulation (3.2.5):** Mensimulasikan logika *routing* di mana pertanyaan berbahaya dialihkan ke manusia.

**Prasyarat:**
* Akun Google Colab.
* Tidak butuh GPU besar (CPU cukup untuk Presidio).

---

## Cara Menjalankan Notebook

Klik *badge* di bawah untuk membuka *notebook* langsung di Google Colab.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hy89aTprVhxQS9BHef2FrKeWJgaiBR7v?usp=sharing)

**Hasil yang Diharapkan:**
Anda akan melihat bagaimana teks *"Halo Budi, NIK saya 3175..."* secara otomatis berubah menjadi *"Halo <PERSON>, NIK saya <US_SSN>..."* (atau entitas lain), siap untuk diproses dengan aman.
