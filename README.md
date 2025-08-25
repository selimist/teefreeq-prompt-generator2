# Uyarlanabilir Prompt Geliştirici

Bu proje, T-shirt tasarım promptlarını kolayca özelleştirmenizi sağlayan interaktif bir web uygulamasıdır.

## Özellikler

- **Dinamik Prompt Oluşturma**: Takım adı, içerik türü ve görsel türü parametrelerine göre otomatik prompt oluşturma
- **Koşullu Mantık**: Seçilen görsel türüne göre farklı prompt bölümlerinin dahil edilmesi
- **Kullanıcı Dostu Arayüz**: Modern ve responsive tasarım
- **Kopyalama ve İndirme**: Oluşturulan promptları kolayca kopyalama ve dosya olarak indirme
- **Form Sıfırlama**: Tek tıkla tüm alanları temizleme

## Teknolojiler

- **React 19**: Modern React hooks ve bileşenler
- **Vite**: Hızlı geliştirme ve build aracı
- **Tailwind CSS**: Utility-first CSS framework
- **shadcn/ui**: Modern UI bileşenleri
- **Lucide React**: İkonlar

## Kurulum

### Yerel Geliştirme

```bash
# Bağımlılıkları yükle
pnpm install

# Geliştirme sunucusunu başlat
pnpm run dev

# Tarayıcıda http://localhost:5173 adresini aç
```

### Production Build

```bash
# Production build oluştur
pnpm run build

# Build'i önizle
pnpm run preview
```

## Vercel'e Dağıtım

Bu proje Vercel'e dağıtım için optimize edilmiştir:

1. GitHub'a projeyi yükleyin
2. Vercel hesabınızda "New Project" seçin
3. GitHub repository'sini seçin
4. Vercel otomatik olarak build ayarlarını algılayacaktır
5. Deploy butonuna tıklayın

### Vercel Ayarları

- **Build Command**: `pnpm run build`
- **Output Directory**: `dist`
- **Install Command**: `pnpm install`

## Kullanım

1. **Takım Adı**: İstediğiniz takım adını girin (örn: Arsenal, Barcelona)
2. **İçerik Türü**: Tasarım konusunu belirleyin (örn: Fans, Players, History)
3. **Görsel Türü**: Slogan veya Grafik seçin
4. **Prompt Oluştur** butonuna tıklayın
5. Oluşturulan promptu kopyalayın veya indirin

## Prompt Şablonu

Uygulama aşağıdaki temel şablonu kullanır:

```
You are a creative T-shirt concept designer.
A realistic mockup of a male model wearing a team-color T-shirt with printed design inspired by {{team}} {{content_type}}.
The T-shirt must not include any official club logos, badges, sponsor names, copyrighted elements, or brand names.
The design should feature {{visual_type}} based on {{content_type}}.

[Koşullu içerik - görsel türüne göre]

The T-shirt color should match {{team}}'s home kit color, with design elements in contrasting tones.

**TASK:** Offer 5 creative design suggestions with short descriptions of the {{visual_type}}.
```

## Katkıda Bulunma

1. Bu repository'yi fork edin
2. Yeni bir branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Değişikliklerinizi commit edin (`git commit -m 'Add some amazing feature'`)
4. Branch'inizi push edin (`git push origin feature/amazing-feature`)
5. Pull Request oluşturun

## Lisans

Bu proje MIT lisansı altında lisanslanmıştır.

