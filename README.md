# Miterra Web - Artisan Coffee Website

Miterra Cafe için modern, responsive bir web sitesi. React + Vite ile geliştirilmiştir.

## 🚀 Özellikler

- ✨ Modern ve responsive tasarım
- 🌙 Dark mode desteği
- 📱 Mobil uyumlu
- 🎨 Tailwind CSS ile stil
- ⚡ Vite ile hızlı geliştirme

## 📦 Kurulum

```bash
# Bağımlılıkları yükle
npm install

# Geliştirme sunucusunu başlat
npm run dev

# Production build oluştur
npm run build

# Build'i önizle
npm run preview
```

## 🌐 GitHub Pages'e Deploy

Bu proje GitHub Actions ile otomatik olarak GitHub Pages'e deploy edilir.

### Adımlar:

1. **Repository oluşturun** (eğer yoksa):
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/KULLANICI_ADI/REPO_ADI.git
   git push -u origin main
   ```

2. **Repository adını `vite.config.js`'de güncelleyin**:
   - `vite.config.js` dosyasındaki `base: '/miterra-web/'` kısmını kendi repository adınızla değiştirin
   - Örnek: Eğer repository adınız `my-cafe-site` ise, `base: '/my-cafe-site/'` yapın
   - Eğer custom domain kullanıyorsanız veya root domain'de yayınlayacaksanız `base: '/'` bırakın

3. **GitHub Pages'i etkinleştirin**:
   - GitHub repository'nize gidin
   - Settings → Pages → Source: "GitHub Actions" seçin

4. **Deploy**:
   - `main` branch'ine push yaptığınızda otomatik olarak deploy başlar
   - Actions sekmesinden deploy durumunu takip edebilirsiniz
   - Deploy tamamlandıktan sonra siteniz `https://KULLANICI_ADI.github.io/REPO_ADI/` adresinde yayında olacak

### Manuel Deploy (Alternatif)

Eğer GitHub Actions yerine manuel deploy yapmak isterseniz:

```bash
npm install --save-dev gh-pages

# package.json'a ekleyin:
# "deploy": "gh-pages -d dist",
# "predeploy": "npm run build"

npm run deploy
```

## 📝 Notlar

- İlk deploy birkaç dakika sürebilir
- GitHub Pages HTTPS kullanır
- Custom domain kullanmak için GitHub Pages ayarlarından domain ekleyebilirsiniz
