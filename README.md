# EKG Ön Yükselteç – Analog Ön Uç PCB Tasarımı

Bu repoda, düşük genlikli EKG sinyallerinin şartlandırılması amacıyla tasarlanan op-amp tabanlı bir analog ön yükselteç devresinin şematik, simülasyon ve PCB tasarım çalışmaları yer almaktadır. Proje eğitim ve laboratuvar uygulamaları için hazırlanmıştır.

## Teknik Özellikler

- Giriş sinyali: µV – mV seviyesinde EKG sinyali  
- Mimari: Çok kademeli analog sinyal şartlandırma  
- Besleme: ±9 V çift kutuplu  

## Sinyal Zinciri

- **Enstrümantasyon Yükselteci (INA128)**
  - Yüksek giriş empedansı
  - Yüksek CMRR
  - İlk kademe diferansiyel kazanç (~11.6)

- **Right Leg Drive (RLD)**
  - Ortak mod gürültü bastırma
  - 50 Hz şebeke parazitinin azaltılması

- **Filtre Katmanları**
  - HPF ≈ 0.05 Hz (DC ofset ve baseline wander bastırma)
  - LPF ≈ 106 Hz (yüksek frekanslı gürültü bastırma)
  - Notch ≈ 50 Hz (şebeke gürültüsü bastırma)

- **Çıkış Yükseltme**
  - Non-inverting op-amp konfigürasyonu

## PCB Tasarımı

- Proteus kullanılarak tasarlanmıştır  
- Analog sinyal yolları kısa tutulmuştur  
- Gürültüye hassas katmanlar güç hatlarından izole edilmiştir  

## Doğrulama

- mV seviyesinde sinüs sinyalleri ile simülasyon  
- Dijital osiloskop ile donanım testleri  
- Simülasyon ve gerçek ölçümler uyumludur  

## Uyarı

Bu çalışma **yalnızca eğitim ve deneysel amaçlıdır**.  
Tıbbi teşhis veya klinik kullanım için uygun değildir.

## Kullanılan Araçlar

- Proteus Design Suite
- Dijital Osiloskop
- Sinyal Jeneratörü
