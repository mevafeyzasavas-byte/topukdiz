# Egzersiz Android Uygulaması

Bu proje, `egzersiz.zip` içindeki HTML sayfalarını (Diz / Topuk Dikeni egzersizleri)
WebView üzerinden gösteren basit bir Android uygulamasıdır. Uygulama ikonu
yüklediğiniz `icon-512.png` dosyasından üretildi.

## GitHub'da APK oluşturma adımları

1. GitHub'da yeni, **boş** bir repo oluşturun (README eklemeden).
2. Bu klasördeki tüm dosyaları o reponun kök dizinine push edin:

   ```bash
   git init
   git add .
   git commit -m "İlk sürüm"
   git branch -M main
   git remote add origin https://github.com/KULLANICI_ADIN/REPO_ADIN.git
   git push -u origin main
   ```

3. Push işleminden sonra GitHub otomatik olarak **Actions** sekmesinde
   `Build APK` iş akışını çalıştırır (yaklaşık 2-4 dakika sürer).
4. İş akışı bitince ilgili çalışmanın (workflow run) sayfasına girin,
   en altta **Artifacts** bölümünden `egzersiz-debug-apk` dosyasını indirin.
   İçinden çıkan `app-debug.apk` telefonunuza kurulabilir APK dosyasıdır.

Not: Bu debug APK'dır, imzasızdır ama Android'de "bilinmeyen kaynaklardan
yükleme" izniyle doğrudan kurulabilir. Play Store'a yüklemek isterseniz
release imzalama adımı ayrıca eklenmelidir, isterseniz onu da ekleyebilirim.
