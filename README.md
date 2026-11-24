# 2.6.11 LAB – Etkinlik Bitiş Saati Hesaplayıcı

Bu proje, **BOZ213** dersi kapsamında Python programlama dilinde temel aritmetik operatörlerin (`+`, `//`, `%`) ve kullanıcı girdi/çıktı fonksiyonlarının (`input()`, `print()`) kullanımını pekiştirmek amacıyla geliştirilmiştir.

Program; kullanıcıdan bir etkinliğin başlangıç saatini (saat ve dakika cinsinden) ve süresini (dakika cinsinden) alarak, etkinliğin 24 saatlik zaman dilimine göre saat kaçta sona ereceğini hesaplar.

## Proje ve Öğrenci Bilgileri

* **Öğrenci:** Mislina Danacı (`MislinaDanaci`)
* **Öğrenci Numarası:** 25040192
* **Ders Kodu:** BOZ213
* **Dosya Adı:** `2.6.11LAB.py`

## Çalışma Mantığı

1. **Veri Girişi:** Kullanıcıdan başlangıç saati (`hour`), başlangıç dakikası (`mins`) ve etkinlik süresi (`dura`) tam sayı (`int`) olarak alınır.
2. **Toplam Dakika Hesabı:** Başlangıç dakikası ile etkinlik süresi toplanır (`toplam_dakika = mins + dura`).
3. **Saat ve Dakika Dönüşümü:**
   * Tam bölme operatörü (`// 60`) ile dakikaların oluşturduğu ek saat (`ekstra_saat`) hesaplanır.
   * Mod alma operatörü (`% 60`) ile kalan bitiş dakikası (`son_dakika`) bulunur.
4. **24 Saat Formatına Uyarlama:** Başlangıç saatine ek saatler eklenir ve gün dönümünü (24 saati aşan durumları) doğru hesaplamak için `24` ile modu alınır (`son_saat = (hour + ekstra_saat) % 24`).
5. **Çıktı:** Hesaplanan bitiş zamanı `saat:dakika` formatında ekrana yazdırılır.

## Kurulum ve Çalıştırma

Bilgisayarınızda **Python 3** kurulu olmalıdır. Projeyi çalıştırmak için terminal veya komut istemcisinde dosya dizinine giderek aşağıdaki komutu çalıştırabilirsiniz:

```bash
python 2.6.11LAB.py
```

## Örnek Kullanım

**Girdi:**
```text
starting time (hours): 12
starting time (minutes): 17
event duration (minutes: 59
```

**Çıktı:**
```text
13:16
```
