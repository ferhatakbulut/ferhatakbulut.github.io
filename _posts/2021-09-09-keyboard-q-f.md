---
layout: post
title: Bilgisayar Açılırken Default Klavye Ayarı Q klavye - F klavye
categories: [genel, klavye, bilgisayar, windows]
tags: [klavye, f, q]
description: Bilgisayar açılıştaki klavye ayarı (F klavye yada Q klavye)
---

Windows işletim sistemi için bilgisayarın açılıştaki klavye ayarı için, yani klavye olarak bilgisayar F klavyede mi yoksa
Q klavyede mi başlatıcak. Onu ayarlamak için

**Çalışıtır** açıyoruz. Çalıtıra **regedit** yazarak kayıt defterine ulaşıyoruz. Daha sonra aşağıdaki resimde bulunan yolu izliyoruz.
Yani **HKEY_USERS -> .DEFAULT -> Keyboard Layout -> Preload** bölümüne kadar gidiyoruz.
Sol menüde bulunan **1** dosyasına çift tıklayacak **Q klavye** için **0000041f** yapıyoruz. **F klavye** için **0001041f** değerini girmemiz yeterli.

<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/klavye.png">



Kolay gelsin.

