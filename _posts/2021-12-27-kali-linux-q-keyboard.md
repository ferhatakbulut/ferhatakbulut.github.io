---
layout: post
title: Kali Linux Q Klavye - Kali Linux Q Keyboard
categories: [linux, kali]
tags: [q, keyboard, klavye]
description: Kali Linux klavye ayarını Q klavye olarak ayarlama işlemi
---

Terminal ekranımızı açıyoruz. Aşağıdaki komut ile klavye ayarlarınız geçici olarak **türkçe** olarak ayarlıyoruz.

{% highlight yaml %}

    setxkbmap tr

{% endhighlight %}

Ama bu komut bilgisayar yeniden başladığında tekrar yazmanız gerekecektir.
Bunun önüne geçmek için her defasında bilgisayar yeniden başladığında komutun otomatik çalışması için aşağıdaki adımları izlememiz yeterlidir.

İlk olarak menüden **Applications -> Settings -> Session and Startup** tıklıyoruz


<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/k1.png">


Daha sonra açılan pencerede **Application Autostart** yani uygulama otomatik başlatma sekmesine geçiyoruz ve sol altta görülen **+** butonuna tıklayın.


<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/k2.png">


Uygulama ekleme kısmında "Name" kısmına istediğiniz bir isim verebilirsiniz. Burada önemli olan "Command" kısmıdır. Buraya **setxkbmap tr** yazıp, 
**Trigger** kısmını da **on login** ayarladıktan sonra **OK** butonuna tıklayın


<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/k3.png">


Bu işlemler ile Kali Linux Türkçe klavye yapma komutunu işletim sistemine giriş (login) yaptıktan sonra otomatik çalışması için ayarladık. 
Bu sayede sistemi kapatıp, tekrar açtığımızda başka işlemler yapmaya gerek kalmadan arkada kendisi kodu işleyecek ve klavyemiz Türkçe olacaktır.

Ayarların aktif olması için bilgisayarı yeniden başlatmanız gerekebilir.

Kolay gelsin.

