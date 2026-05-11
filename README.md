# Muki ISO 🚀

Ovo je modifikovana verzija **Windows 10 Pro 22H2** optimizovana za maksimalne performanse

Fokus na eliminaciju nepotrebnih servisa i telemetrije uz zadržavanje stabilnosti sistema

## ✨ Opis
Sistem je prilagođen za:
- **Svakodnevni rad:** Brz odziv UI-a i minimalna potrošnja RAM-a/procesora
- **Gaming:** Smanjen input lag, optimizovan mrežni stack i stabilniji FPS

## 📥 Download
[ ![Download Muki Pro](https://img.shields.io/badge/Download-Muki_Pro_ISO-blue?style=for-the-badge&logo=google-drive) ](https://drive.google.com/uc?export=download&id=1F4IspALWMuhKj9kkO_P8HVtJ3wDc-dvi)

*Napomena: Zbog veličine fajla (3.3GB),

Google Drive će prikazati poruku da ne može skenirati fajl na viruse. 

Samo kliknite na **"Download anyway"**.*

## 🛠️ Instalacija
Odaberite jedan od dva načina za pokretanje instalacije:

---

### 🟢 NAČIN A: Preko USB Flash-a

**1. Priprema USB-a:**
- Koristite **Rufus**
- Kliknite na **SELECT** i odaberite **Muki LZX 10.iso**
- Sve opcije će se automatski postaviti (GPT/UEFI)

**2. BIOS Postavke (Obavezno!):**
Da bi sistem radio ispravno, u BIOS-u podesite sljedeće:
- Obavezno **ISKLJUČITE CSM** (koristite isključivo UEFI mod)
- Obavezno **ISKLJUČITE Secure Boot**

**3. Pokretanje:**
- Restartujte PC i stiskajte taster za Boot Menu (F12, F11, F8 ili Del...)
- Odaberite vaš USB

### 🔵 Preko postojećeg sistema (Recovery)

- Idite na: **Settings** -> **Update & Security** -> **Recovery**
- Pod **Advanced startup** kliknite **Restart now**
- Kada se pojavi plavi meni, idite na **Use a device** i odaberite vaš **USB**

---

### 💠 NAČIN B: Hirurška instalacija bez USB-a (Direktno iz ISO-a)

Instaliraš novi sistem na malu particiju, a onda ga proširiš na cijeli disk

## 1. Priprema particije:

Desni klik na Start -> Disk Management

Desni klik na tvoju najveću particiju -> Shrink Volume

Unesi 50000 (50GB) i klikni Shrink

Od tog crnog prostora napravi novu particiju (New Simple Volume), formatiraj je kao NTFS i dodijeli joj slovo (npr. X:)

## 2. Podešavanje u WinNTSetup alatu:

Pokreni WinNTSetup

Gornje polje (Installation files): Klikni Search i jednostavno odaberi tvoj Muki LZX.iso fajl. Alat će sam prepoznati sistem unutar njega

Srednje polje (Boot drive): Odaberi postojeću EFI particiju (obično 100MB, FAT32, označena zelenom ikonicom)

Donje polje (Installation drive): Odaberi novu particiju koju si napravio od 50GB (X:)

Važno: Desno pod "Option" označi "Drive letter preassignment" i postavi na C:. Tako će novi sistem znati da je on glavni

Klikni Setup -> OK

## 3. Prelazak na novi sistem:

Restartuj PC. Na ekranu za izbor sistema odaberi svoj novi Windows

Kada uđeš u novi sistem, instaliraj osnovne drajvere (AMD drajver za RX 6500 XT)

## 4. Brisanje starog Windowsa i spajanje diska:

Sada kada si u novom sistemu, otvori Disk Management

Desni klik na particiju gdje je bio stari Windows (koja ti sad stoji kao višak) -> Format

Da bi spojio tih 50GB sa ostatkom diska u jedan veliki C:, koristi MiniTool Partition Wizard

U njemu uradi desni klik na C: (50GB) -> Extend -> izvuci klizač do kraja da "proguta" formatiranu particiju

Klikni Apply i pusti ga da završi nakon restarta


## 📜 Post-Install Skripte
Nakon prvog restarta dočekat će vas automatizovana **instalacija za Brave**
- **PAŽLJIVO ČITAJTE** sve naredbe koje skripta ispisuje u konzoli
- Nemojte gasiti prozor SKRIPTA SE SAMA BRISE

## ⚠️ Napomena
Ovaj ISO je pravljen za maksimalne performanse i niske latencije

Neke Windows funkcije su trajno uklonjene Koristite na vlastitu odgovornost

— autor nije odgovoran za bilo kakvu štetu nastalu nepravilnim korištenjem ili nekompatibilnošću hardvera

## 📄 Licenca
Ovaj projekt je licenciran pod [MIT Licencom](LICENSE)

---
**Enjoy your low latency experience!** 🎮
