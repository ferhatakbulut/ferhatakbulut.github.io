---
layout: post
title: Arduino ile ilk başlangıç
categories: [Genel,Arduino]
tags: [arduino]
description: Arduino Dersleri ve Bazı Kod Yapılarının Anlatımları
---

Örnek arduino kartı ve üzerinde segment ledi ile bir örnek resmi üzerinde gösterilmektedir. Kablolalama ile pin sırasına göre
segment ledine kart üzerinde bağlatılar şekildeki gibi yapılır. Ayrıca **5V** ile anot kutuplarına bağlanır.

<img src="https://raw.githubusercontent.com/ferhatakbulut/ferhatakbulut.github.io/main/image/ar1.png">


{% highlight yaml %}

int a=4;
int b=5;
int c=6;
int d=7;
int e=8;
int f=3;
int g=2;

{% endhighlight %}

pinlerin segmentin hangi değerlerine atandığını göstermekdir.

{% highlight yaml %}

void setup()
{
  pinMode(a,OUTPUT);
  pinMode(b,OUTPUT);
  pinMode(c,OUTPUT);
  pinMode(d,OUTPUT);
  pinMode(e,OUTPUT);
  pinMode(f,OUTPUT);
  pinMode(e,OUTPUT);
  pinMode(g,OUTPUT);
}

{% endhighlight %}

Pinlere ışık verilmesi gerektiğini gösteren kod yapısıdır.

{% highlight yaml %}

void setup()
{
  digitalWrite(a,LOW);
}

{% endhighlight %}

Segmentteki ledi yak demek

{% highlight yaml %}

void setup()
{
  digitalWrite(b,HIGH);
}

{% endhighlight %}

Segmentteki ledi söndür demek

{% highlight yaml %}

 delay(1000);

{% endhighlight %}

1 saniye bekle demek.


Kolay gelsin
