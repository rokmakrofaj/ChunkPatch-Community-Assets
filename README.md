# ChunkPatch Community Assets

Bu depo, topluluk tarafından hazırlanan Türkçe yamaların ChunkPatch Launcher'da yayınlanabilmesi için oluşturulmuştur.

Katkıda bulunmak istiyorsanız aşağıdaki adımları takip edin.

---

# Nasıl Katkıda Bulunurum?

## 1. Repository'yi Fork'layın

Sağ üst köşedeki **Fork** butonuna tıklayarak depoyu kendi GitHub hesabınıza kopyalayın.

---

## 2. Türkçe Yamanızı Hazırlayın

Yamanızı **ZIP** formatında hazırlayın.

Dosya adının aşağıdaki standartlardan birine uyması gerekir.

Örnekler:

```
outlast-steam.zip
outlast-2-steam.zip
outlast-2-epic.zip
far-cry-5-steam.zip
elden-ring-steam.zip
```

Dosya adlarında yalnızca:

- Küçük harf
- Rakam
- `-` karakteri

kullanılmalıdır.

---

## 3. community-database.json Dosyasını Güncelleyin

Dosyanın sonuna aşağıdaki formata uygun yeni bir kayıt ekleyin.

```json
{
  "game": "Far Cry 5",
  "game_id": "552520",
  "name": "Far Cry 5 – Tam Türkçe Çeviri",
  "description": "Türkçe yamanız hakkında kısa açıklama.",
  "author": "GitHub kullanıcı adınız",
  "version": "1.0.0",
  "date": "2026-08-04",
  "progress": 100,
  "platform": "Steam",
  "verified": false,
  "download_url": "",
  "cover": ""
}
```

### Alan Açıklamaları

| Alan | Açıklama |
|------|----------|
| `game` | Oyun adı |
| `game_id` | Steam App ID |
| `name` | Yama adı |
| `description` | Kısa açıklama |
| `author` | GitHub kullanıcı adınız veya ekip adınız |
| `version` | Yama sürümü |
| `date` | Yayın tarihi (`YYYY-MM-DD`) |
| `progress` | Çeviri yüzdesi (0-100) |
| `platform` | Steam, Epic Games, Ubisoft Connect vb. |
| `verified` | **false** olarak bırakılmalıdır |
| `download_url` | **Boş bırakılmalıdır** |
| `cover` | İsteğe bağlı (boş bırakabilirsiniz) |

---

## 4. Pull Request Açın

ZIP dosyanızı ve güncellenmiş `community-database.json` dosyasını gönderdikten sonra bir **Pull Request** oluşturun.

---

# İnceleme Süreci

Gönderilen tüm katkılar manuel olarak incelenir.

Kontrol edilen başlıca kriterler:

- Dosya bütünlüğü
- Zararlı yazılım kontrolü
- JSON doğruluğu
- Çeviri kalitesi
- Dosya isimlendirme standardı

İnceleme tamamlandıktan sonra uygun görülen yamalar:

- ✅ GitHub Releases'e yüklenir.
- ✅ `download_url` alanı güncellenir.
- ✅ `verified` değeri **true** olarak değiştirilir.
- ✅ ChunkPatch Launcher üzerinden yayınlanır.

---

# Önemli Kurallar

- ZIP dışındaki arşiv formatları kabul edilmez.
- Şifreli arşivler kabul edilmez.
- Zararlı yazılım içeren dosyalar reddedilir.
- `verified` alanını değiştirmeyin.
- `download_url` alanını boş bırakın.
- Dosya adlarını standartlara uygun hazırlayın.

---

# Teşekkürler ❤️

ChunkPatch'e katkıda bulunduğunuz için teşekkür ederiz.

Topluluğun desteği sayesinde daha fazla oyunu Türkçe oynayabiliyoruz.
