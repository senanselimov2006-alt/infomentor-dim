# InfoMentor — DİM informatika AI müəllimi (parolsuz giriş)

Sayt açıldıqda istifadəçidən ayrıca hesab, qeydiyyat və ya parol istənməyəcək. Linki olan hər kəs sayta daxil ola bilər.

## Render Free-də yayımlama

1. ZIP faylını aç.
2. GitHub-da yeni repository yarat. Repository-ni **Private** saxlaya bilərsən.
3. Layihənin içindəki faylları GitHub repository-sinə yüklə.
4. https://render.com/ saytında qeydiyyatdan keç və GitHub hesabını qoş.
5. Render Dashboard → **New** → **Web Service** seç və repository-ni qoş.
6. Bu parametrləri daxil et:
   - Runtime: Node
   - Build Command: `npm install`
   - Start Command: `npm start`
   - Instance Type: Free
7. Environment bölməsində əlavə et:
   - `OPENAI_API_KEY` = şəxsi OpenAI API açarın
   - `AI_MODEL` = `gpt-4.1-mini` (istəyə bağlı)
8. **Create Web Service** seç. Deploy bitəndə Render sənə `https://...onrender.com` formasında link verəcək.
9. Həmin linki Android telefonda və kompüterdə aç. Sayt parol və qeydiyyat istəməyəcək.

## Vacib qeydlər

- Sayt parolsuz və ictimai linklə açıq olacaq. Linki alan başqa şəxslər də istifadə edə bilər.
- GitHub repository-si Private qala bilər; bu, yayımlanmış saytın linkini gizli etmir.
- API açarını yalnız Render-in Environment bölməsinə yaz. Onu GitHub-a, HTML/JS fayllarına və ya çat mesajına göndərmə.
- Render Free xidməti müəyyən müddət fəaliyyətsiz qaldıqda yuxuya gedə bilər; ilk açılış bir qədər gecikə bilər.
- AI sorğuları üçün OpenAI API istifadəsi ayrıca ödəniş yarada bilər.
- Öyrənmə irəliləyişi brauzerin localStorage yaddaşında saxlanır; cihazlar arasında avtomatik sinxronlaşmır.

## Lokal sınaq

Node.js 18+ tələb olunur:
```bash
npm install
```
Sonra `OPENAI_API_KEY` mühit dəyişənini təyin edib:
```bash
npm start
```
Brauzerdə `http://localhost:3000` aç.
