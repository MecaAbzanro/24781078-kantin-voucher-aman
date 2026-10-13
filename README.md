# Kantin Voucher — Web Aman (Mitigasi Prompt Injection)

Praktikum **P06: Risiko AI LLM dan Prompt Injection**

## Identitas Mahasiswa
- **Nama**: M.Putara Meca Abzanro
- **NIM**: 24781078
- **Kelas / Praktikum**: P06 - Risiko AI LLM dan Prompt Injection

---

## Deskripsi Singkat
Repositori ini berisi aplikasi web simulasi kasir & asisten chatbot kantin yang telah **dilindungi dari serangan Prompt Injection**.

### Mekanisme Pertahanan (Mitigasi):
1. **Input Validation & Filtering**: Deteksi berbasis pola/regex terhadap kata kunci injeksi (*jailbreak*, *override*, *kamu kasir*, *diskon 100%*, *ignore previous*).
2. **Hardened System Prompt**: Guardrails ketat yang membatasi peran AI hanya sebagai penyedia informasi menu & harga, bukan kasir penerbit voucher.
3. **Penyangkal Otomatis**: Setiap percobaan manipulasi langsung ditolak secara aman tanpa membocorkan sistem internal.
4. **Offline Secure Simulation**: Mode simulasi aman tetap memvalidasi input meskipun pengujian dilakukan tanpa API key.

---

## Cara Menjalankan
1. Buka file `index.html` secara langsung di browser, atau
2. Jalankan via live server / static web hosting (GitHub Pages, Netlify, Vercel).
3. Anda dapat memasukkan API Key OpenRouter jika ingin pengujian dengan model langsung, atau langsung mencoba dalam mode simulasi interaktif.
