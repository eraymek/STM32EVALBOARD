# 🚀 Çok Yönlü Endüstriyel STM32 Geliştirme Kartı

Bu geliştirme kartı; endüstriyel otomasyon, Ar-Ge projeleri, otonom sistemler ve hassas motor kontrolü uygulamalarında kullanılmak üzere, farklı sektörlerin ihtiyaçlarına cevap verebilecek esneklikte ve çok yönlü olarak tasarlanmıştır.

Tasarım süreci **Altium Designer** ortamında endüstriyel standartlara uygun olarak gerçekleştirilmiş olup; güç bütünlüğü, haberleşme güvenilirliği ve elektriksel koruma önlemleri dikkate alınmıştır.

---

## 🎯 Uygulama Alanları
Bu geliştirme kartı, barındırdığı zengin çevre birimleri sayesinde aşağıdaki alanlarda doğrudan kullanılabilir:
* 🏭 **Akıllı Üretim Sistemleri:** Fabrika otomasyonu, robotik kollar ve sensör tabanlı kontrol sistemleri.
* 🌐 **IoT ve Akıllı Cihazlar:** Akıllı ev/bina çözümleri, enerji yönetimi ve güvenlik uygulamaları.
* ⚕️ **Medikal Teknolojiler:** Hassas ölçüm, veri işleme ve kontrol gerektiren medikal cihazlar.
* ⚡ **Enerji Sistemleri:** Yenilenebilir enerji projeleri ve güç takip sistemleri.
* 🔬 **Eğitim ve Ar-Ge:** Üniversite projeleri, hızlı prototipleme (rapid prototyping) ve test platformları.
* 🤖 **Hassas Motor Kontrolü:** CNC makineleri, 3D yazıcılar ve otonom araç/robot sistemleri.

---

## 🛠️ Tasarım ve Teknik Spesifikasyonlar

### 🧠 Merkezi İşlem Birimi (CPU)
* **Mikrodenetleyici:** STM32F373RCT (ARM Cortex-M4)
* **Kapasite:** 256 KB Flash, 32 KB RAM
* **Arayüzler:** 51 adet yapılandırılabilir I/O pini; USART, I2C, SPI ve CAN Bus donanımsal haberleşme desteği.

### 🔌 Güç Yönetimi (Power Supply)
* **Geniş Giriş Gerilimi:** 12V - 24V DC endüstriyel besleme giriş aralığı.
* **Kademeli Regülasyon:**
  * **LM2576 (Buck Converter):** 12-24V giriş gerilimini yüksek verimle 5V'a düşürür.
  * **LD1117 (LDO Regülatör):** 5V gerilimi, MCU ve lojik seviyeler için stabil 3.3V'a regüle eder.

### 📡 İletişim ve Haberleşme
* **Endüstriyel Haberleşme:** Modbus RTU protokolü ile tam uyumlu **MAX485 (RS-485)** haberleşme devresi (Uzun mesafe ve gürültülü ortamlar için güvenilir veri aktarımı).

### 🎛️ Analog ve Dijital Sinyal İşleme
* **Analog İşlem:** ADC/DAC dönüştürücü sinyalleri için **LMV358** Op-Amp entegrasyonu.
* **Dijital Yönlendirme:** Çift yönlü sinyal izolasyonu ve buffer (tampon) işlemi için **74HCT245** lojik entegresi.

### 💾 Hafıza (Memory) Birimleri
* **Harici Flash:** 8 Mbit SST25 (Veri loglama ve kapsamlı parametre saklama).
* **EEPROM:** 64 Kbit M24C64 (Elektrik kesintilerinde kalıcı olması gereken kritik konfigürasyon verileri için).

### 🖥️ Kullanıcı Arayüzü
* **Ekran:** Sistem durumunu ve sensör verilerini izlemek için LCD ekran portu.
* **Kontrol:** Cihaz üzerinden manuel parametre girişi ve menü kontrolü sağlamak amacıyla 6 adet fiziksel buton (Debounce korumalı).

---
