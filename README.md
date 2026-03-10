<p align="center">
  <a href="http://makeapullrequest.com"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg"></a>
  <img src="https://img.shields.io/badge/os-linux-brightgreen">
  <img src="https://img.shields.io/badge/os-mac-brightgreen">
  <img src="https://img.shields.io/badge/os-android-brightgreen">
  <img src="https://img.shields.io/badge/os-windows-yellowgreen">
</p>

<h1 align="center">ani-cli</h1>

<p align="center">
  Terminalde anime arama, izleme ve indirme aracı.
</p>

---

## Proje Hakkında

**ani-cli**, terminal üzerinden anime aramanıza, izlemenize ve indirmenize olanak tanıyan bir shell scriptidir. [allmanga.to](https://allmanga.to/) sitesinden içerik çeker ve `mpv`, `fzf` gibi araçlarla entegre çalışır. Arkadaşlarınızla senkronize izleme (syncplay) desteği de sunar.

### Öne Çıkan Özellikler

- 🔍 Anime arama ve bölüm seçimi (fzf arayüzü ile)
- ▶️ mpv veya VLC ile doğrudan oynatma
- 📥 Bölüm veya seri indirme (`-d` bayrağı)
- 🎌 Dub/sub seçeneği (`--dub`)
- 🔁 Giriş/çıkış sekanslarını otomatik atlama (ani-skip ile)
- 🖥️ Linux, macOS, Android, Windows ve iOS desteği
- 🔄 Kendini güncelleme (`ani-cli -U`)

---

## Kurulum

Platforma göre kurulum için lütfen [orijinal proje sayfasını](https://github.com/pystardust/ani-cli) ziyaret edin.

### Hızlı Kurulum (Kaynak)

```sh
git clone "https://github.com/pystardust/ani-cli.git"
sudo cp ani-cli/ani-cli /usr/local/bin
rm -rf ani-cli
```

### Bağımlılıklar

| Araç | Amaç |
|------|------|
| `curl` | HTTP istekleri |
| `fzf` | Kullanıcı arayüzü |
| `mpv` | Video oynatıcı |
| `ffmpeg` | m3u8 indirici (yedek) |
| `yt-dlp` | m3u8 indirici |
| `aria2c` | İndirme yöneticisi |
| `patch` | Kendini güncelleme |

---

## Kullanım

```sh
ani-cli [seçenekler] [anime adı]
```

| Bayrak | Açıklama |
|--------|----------|
| `-d` | İndir |
| `-e <bölümler>` | Bölüm aralığı (ör: `1-12`) |
| `-q <çözünürlük>` | Kalite seç (ör: `1080`) |
| `--dub` | Dublaj izle |
| `--vlc` | VLC ile oynat |
| `-U` | Güncelle |
| `-h` | Yardım |

---

## Sorun Giderme

Eğer `No results found` hatası alıyorsanız önce aracı güncelleyin:

```sh
# Linux / Mac / Android
sudo ani-cli -U

# Windows
ani-cli -U
```

Sorun devam ederse [Issue açın](https://github.com/pystardust/ani-cli/issues).

---

## Teşekkür ve Atıf

Bu proje **[pystardust](https://github.com/pystardust)** tarafından oluşturulmuştur.

Projeye katkıda bulunanlar:
[port19x](https://github.com/port19x) · [CoolnsX](https://github.com/CoolnsX) · [justchokingaround](https://github.com/justchokingaround) · [Derisis13](https://github.com/Derisis13) · [71zenith](https://github.com/71zenith) · [ykhan21](https://github.com/ykhan21)

Orijinal kaynak kodu ve tam katkıcı listesi için:
👉 [github.com/pystardust/ani-cli](https://github.com/pystardust/ani-cli)

---

## Lisans

Bu proje [GPL-3.0](./LICENSE) lisansı altında dağıtılmaktadır.
