# Dolphin Service Menu - SHA-1 Hash Tool

[English](#english) | [Türkçe](#türkçe)

---

## English

A lightweight KDE Dolphin Service Menu that calculates and displays the SHA-1 checksum of any file directly from the context menu and automatically copies it to your clipboard.

![License](https://img.shields.io/badge/License-GPLv3-blue.svg)
![KDE Plasma](https://img.shields.io/badge/KDE-Plasma%205%20%2F%206-blueviolet.svg)

### Features
- **One-click calculation:** Compute SHA-1 hash directly from Dolphin's right-click menu.
- **Auto-clipboard:** Automatically copies the calculated hash value to your clipboard.
- **Display dialog:** Shows the result in a clean `kdialog` window for easy verification.
- **X11 & Wayland support:** Works seamlessly on both display servers using `xclip` or `wl-clipboard`.
- **Clean integration:** Top-level context menu entry with no nested submenu clutter.

### Prerequisites & Dependencies
Ensure the following packages are installed on your system:
- `kdialog` (KDE Dialog display utility)
- `xclip` (for X11 session clipboard support) or `wl-clipboard` (for Wayland session clipboard support)

#### Installing dependencies

**Pisi Linux:**
```bash
sudo pisi it kdialog xclip
```

**Arch Linux / Manjaro:**
```Bash
sudo pacman -S kdialog xclip wl-clipboard
```

**Fedora:**
```Bash
sudo dnf install kdialog xclip wl-clipboard
```
**Ubuntu / Debian:**
```Bash
sudo apt install kdialog xclip wl-clipboard
```

**Installation**

*Clone the repository:*
```Bash
git clone [https://github.com/username/dolphin-sha1-servicemenu.git](https://github.com/username/dolphin-sha1-servicemenu.git)

cd dolphin-sha1-servicemenu

Copy the service menu file:

mkdir -p ~/.local/share/kio/servicemenus
cp show-sha1.desktop ~/.local/share/kio/servicemenus/
chmod +x ~/.local/share/kio/servicemenus/show-sha1.desktop

Restart Dolphin:

killall dolphin && dolphin &
```
## Türkçe
Herhangi bir dosyanın SHA-1 doğrulama kodunu (checksum) doğrudan sağ tık menüsünden hesaplayan, ekranda gösteren ve otomatik olarak panoya kopyalayan hafif bir KDE Dolphin Servis Menüsüdür.

**Özellikler**

Tek tıkla hesaplama: Dolphin sağ tık menüsünden doğrudan SHA-1 değerini alın.

Otomatik kopyalama: Hesaplanan hash değerini anında panoya (clipboard) kopyalar.

Açılır pencere: Değeri rahatça görebilmeniz için temiz bir kdialog penceresi sunar.

X11 ve Wayland desteği: xclip veya wl-clipboard kullanarak her iki görüntü sunucusunda da sorunsuz çalışır.

Sade entegrasyon: Alt menü kalabalığı yaratmadan doğrudan ana sağ tık menüsüne yerleşir.

**Gereksinimler ve Bağımlılıklar**

Sisteminizde aşağıdaki paketlerin kurulu olduğundan emin olun:

kdialog (KDE iletişim penceresi aracı)

xclip (X11 panosu için) veya wl-clipboard (Wayland panosu için)

**Bağımlılıkların Kurulumu**

**Pisi Linux:**
```Bash
sudo pisi it kdialog xclip wl-clipboard
```
**Arch Linux / Manjaro:**
```Bash
sudo pacman -S kdialog xclip wl-clipboard
```
**Fedora:**
```Bash
sudo dnf install kdialog xclip wl-clipboard
```
**Ubuntu / Debian:**
```Bash
sudo apt install kdialog xclip wl-clipboard
```
**Kurulum**

*Depoyu klonlayın:*

```Bash
git clone [https://github.com/username/dolphin-sha1-servicemenu.git](https://github.com/username/dolphin-sha1-servicemenu.git)

cd dolphin-sha1-servicemenu

Servis menüsü dosyasını kopyalayın:

mkdir -p ~/.local/share/kio/servicemenus

cp show-sha1.desktop ~/.local/share/kio/servicemenus/

chmod +x ~/.local/share/kio/servicemenus/show-sha1.desktop

*Dolphin'i yeniden başlatın:*

killall dolphin && dolphin &
```
License / Lisans
Distributed under the GNU General Public License v3.0 (GPLv3).
