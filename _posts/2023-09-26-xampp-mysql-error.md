---
layout: post
title: Xampp Mysql Hatası
categories: [Genel,Çözüm,Xampp,Mysql,Hata]
tags: [hata,xampp,mysql,hata]
description: Error Mysql shutdown unexpectedly. This may be due to a blocked port missing dependencies improper privileges a crash, or a shutdown by another method.
---

Xampp başlatıktan sonra mysql başlatınca böyle bir hata verirse yapmamız gereken eski dosyaları temizlemek olacak.
Bunun için yapmamız gerekenler **C:\xampp\mysql** dizinine gidiyoruz. Sonra bu dizinde **data** dizininin bir kopyasını alıyoruz.
Sorun olursa diye yedeğimiz olsun.

<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/x1.png">

Daha sonra **data** dizinine gidiyoruz ve 

1- performance_schema
2- phpmyadmin
3- test

bu dizinleri siliyoruz ve aşağıya doğru tüm dosyaları sadece **ibdata1** dosyası hariç hepsini siliyoruz.


<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/x2.png">

Sonra **C:\xampp\mysql** dizinine gidiyoruz ve **backup** dizinine gidiyoruz ve **ibdata1** hariç herşeyi kopyalıyoruz

<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/x2.png">

ve **C:\xampp\mysql\data** dizinine kopyalıyoruz.
Artık xampp başlatıktan sonra mysql sorunsuz çalıştırabiliriz.

Kolay gelsin.

