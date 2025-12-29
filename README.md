# Phantom SoC (Kapasite Sahtekârlığı) Simülasyonu

Bu projede elektrikli araç şarj altyapısında görülebilecek
Phantom SoC (State of Charge Manipulation) saldırısı
uygulamalı olarak simüle edilmiştir.

## Senaryo
- EV gerçek batarya doluluk oranını gönderir (%60)
- MITM saldırganı bu değeri ağ üzerinde değiştirir (%90)
- CSMS bu tutarsızlığı tespit eder ve şarj oturumunu durdurur

## Bileşenler
- ev.py : Elektrikli araç simülasyonu
- mitm.py : MITM (Man-in-the-Middle) saldırı simülasyonu
- csms.py : Merkezi Şarj Yönetim Sistemi (CSMS)

## Çalıştırma Adımları
Terminalde sırasıyla:

```bash
python csms.py
python mitm.py
python ev.py
