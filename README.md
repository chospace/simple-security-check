# security-check

Cek security headers website-mu. Gratis, tanpa daftar.

🔗 **Live:** https://chospace.github.io/simple-security-check/

## Yang dicek

- ✅ HTTPS aktif atau nggak
- 🛡️ Strict-Transport-Security (HSTS)
- 🛡️ X-Frame-Options / frame-ancestors (anti-clickjacking)
- 🛡️ X-Content-Type-Options (anti MIME-sniffing)
- 🛡️ Content-Security-Policy (anti XSS)
- 🛡️ Referrer-Policy
- 🛡️ Permissions-Policy
- 🔍 Server info disclosure (Server / X-Powered-By header)

## Skor

Mulai dari 100, minus 15 per item gagal, minus 7 per item waspada. Grade A+ sampai F.

## Cara kerja

Halaman statis (HTML + JS + CSS, tanpa framework). Scan via [HackerTarget HTTP Headers API](https://hackertarget.com/http-headers/) yang support CORS — jadi semua jalan di browser, tanpa backend.

## Jalankan lokal

Buka `index.html` langsung di browser, atau:

```bash
python3 -m http.server 8000
# buka http://localhost:8000
```

## Share hasil

Tambahin `?url=contoh.com` di URL buat auto-scan + shareable link.

---

Dibuat oleh [chospace](https://chospace.github.io) 🔒
