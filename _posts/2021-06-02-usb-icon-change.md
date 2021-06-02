---
layout: post
title: USB icon değiştirme (USB icon change)
categories: [genel, usb]
tags: [icon, usb]
description: Kullandığınız USB nin iconunu değiştirebilirsiniz. İstediğiniz bir resim atayabilirsiniz.
---

Yapmanız gerek çok basit.
1-Text dosyasını açıp. Aşağıdaki kodları text dosyasına atıp text dosyasını **autorun.inf** olarak kaydediyoruz.

{% highlight yaml %}

   [AUTORUN]
   label=ferhat
   icon=resim.ico

{% endhighlight %}

2-İcon olarak belirlediğiniz resmi 256x256 olarak boyutunu ayarlayınız.
3-Dosya uzantısı olarak **.ico** olarak belirliyoruz.
4-İcon olarak belirlediğimiz resmide ve **autorun.inf** dosyasını usb mizin içerisine atıyoruz.
5-Tüm bu işlemlerden sonra USB mizi çıkarıp tekrar takmamız yeterlidir.

**NOT:** Bu işlemi bilgisayarın harddisleri içinde uygulayabilirsiniz ;)

Kolay gelsin.

