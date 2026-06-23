# G2 — Kurumsal Doğrulama Siteleri

Bu repo, **G2 doğrulama süreci** için hazırlanmış tek-sayfalık kurumsal/ürün sitelerini içerir.
Amaç tasarım değil; G2 doğrulayıcısına **şirket → marka → ürün → uygulama → domain** ilişkisini
tüm sitelerde **birebir aynı ifadelerle** kanıtlamaktır.

## Kurumsal Zincir

```
VİZYON MRKT YAZILIM VE BİLİŞİM SANAYİ VE TİCARET LİMİTED ŞİRKETİ   (çatı / ana şirket)
        │   MERSİS 0925126047100001 · Vergi No 9251260471
        ▼
WIN Markets  (marka — Vizyon MRKT'nin markası)
        │
        ├── Borsa Robotu  → https://borsarobotu.app/        → App Store id6760553279
        └── Altın Robotu  → https://www.altinrobotu.com/    → App Store id6767850256
```

## Klasörler (her biri ayrı domain / ayrı tek-sayfa site)

| Klasör | Domain | Rol |
|--------|--------|-----|
| `vizyonmrkt/` | vizyonmrkt.com | Çatı şirket (kurumsal) |
| `winmarkets/` | winmarkets.dev | Marka |
| `borsarobotu/` | borsarobotu.app | Ürün |
| `altinrobotu/` | altinrobotu.com | Ürün |

## Yayınlama (Vercel)

Her klasör **ayrı bir Vercel projesi** olarak yayınlanır:
- Vercel → New Project → bu repo → **Root Directory** = ilgili klasör (örn. `vizyonmrkt`)
- Framework: Other / None. İlgili domaini projeye bağla.

## Doğrulanması/güncellenmesi gerekenler (gerçek veri)

- **Telefon numaraları** sitelerde placeholder olarak işaretlendi — gerçek numarayı gir.
- **E-posta adresleri** domain bazlı varsayıldı (info@vizyonmrkt.com vb.) — gerçek kutuları teyit et.
- borsarobotu / altinrobotu ürün domainlerinde zaten canlı kayıt siteleri var; buradaki
  sürümler G2 odaklı kurumsal-zincir vurgulu sürümlerdir. Hangisinin canlıya çıkacağına karar ver.
