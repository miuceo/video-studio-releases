# Video Studio

Mavzu yozing, Video Studio esa u bo‘yicha ovozli, animatsiyali tushuntiruvchi video yaratib beradi
(3Blue1Brown uslubida). Ssenariyni Gemini AI yozadi, animatsiyalar Manim bilan kompyuteringizda
chiziladi. O‘zbek, ingliz va rus tillarida ishlaydi.

Bu repoda faqat o‘rnatish fayllari turadi.

## Yuklab olish

**[Windows uchun yuklab olish (64-bit)](https://github.com/miuceo/video-studio-releases/releases/latest/download/Video-Studio-setup.exe)**

Talablar: Windows 10 yoki 11 (64-bit), birinchi ishga tushirishda internet va ~1.5 GB bo‘sh joy.

## O‘rnatish

1. `Video-Studio-setup.exe` ni ishga tushiring.
2. Windows **"Windows protected your PC"** desa: **More info → Run anyway** ni bosing
   (o‘rnatish fayli hozircha raqamli imzosiz).
3. Ilova birinchi marta ochilganda **"Komponentlarni yuklash va o‘rnatish"** tugmasini bosing
   (Python, Manim, FFmpeg avtomatik o‘rnatiladi, 2–5 daqiqa).
4. Bepul Gemini API kalitini oling: [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
   → **Create API key** → nusxalab ilovaga joylang. Kalit faqat sizning kompyuteringizda,
   Windows Credential Manager’da saqlanadi.
5. **"Barcha tekshiruvlarni boshlash"** — hammasi ✓ bo‘lsa, video yaratishingiz mumkin.

## Bepul limit

Har bir foydalanuvchi o‘z kalitidan foydalanadi. Bepul Gemini limiti bilan kuniga taxminan
3–4 ta qisqa (1–3 daqiqalik) video yaratish mumkin. Google limitlarni o‘zgartirishi mumkin.

## Fayl butunligini tekshirish

PowerShell’da:

```powershell
Get-FileHash .\Video-Studio-setup.exe -Algorithm SHA256
```

Natija release’dagi `SHA256SUMS.txt` bilan bir xil bo‘lishi kerak.
