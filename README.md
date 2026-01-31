# EKG Ön Yükselteç – Analog Ön Uç PCB Tasarımı

Bu projede, düşük genlikli EKG sinyallerinin şartlandırılması için op-amp tabanlı bir analog ön yükselteç devresi tasarlanmış, simülasyonu yapılmış ve PCB uygulaması gerçekleştirilmiştir. Çalışma, analog sinyal işleme ve PCB tasarım prensiplerini uygulamalı olarak ele almaktadır.

## Devre Şeması
<p align="center">
  <img src="images/schematic.png" width="600">
</p>

Devre; INA128 enstrümantasyon yükselteci, Right Leg Drive (RLD) katmanı ve aktif filtre bloklarından oluşmaktadır.

## Teknik Özellikler

- Giriş sinyali: µV – mV seviyesinde EKG sinyalleri  
- Besleme: ±9 V çift kutuplu  
- Enstrümantasyon yükselteci: INA128  
- Filtreleme:
  - HPF ≈ 0.05 Hz  
  - LPF ≈ 106 Hz  
  - Notch ≈ 50 Hz  

## PCB Yerleşimi
<p align="center">
  <img src="images/pcb_layout.png" width="600">
</p>

PCB tasarımında analog sinyal yolları kısa tutulmuş, gürültüye hassas katmanlar güç hatlarından ayrılmıştır.

## 3B Kart Görünümü
<p align="center">
  <img src="images/pcb_3d.png" width="500">
</p>

3B model, bileşen yerleşimi ve mekanik uyumu doğrulamak amacıyla oluşturulmuştur.

## Doğrulama

Devre, mV seviyesinde sinüs sinyalleri ile simüle edilmiş ve dijital osiloskop kullanılarak test edilmiştir. Ölçüm sonuçları simülasyon ile uyumludur.

## Uyarı

Bu çalışma **yalnızca eğitim ve deneysel amaçlıdır**.  
Tıbbi teşhis veya klinik kullanım için uygun değildir.

## Kullanılan Araçlar

- Proteus Design Suite
- Dijital Osiloskop
- Sinyal Jeneratörü
