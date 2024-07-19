---
layout: post
title: Javascript var ve let değişken tanımlama farkı
categories: [Genel,Çözüm,Javascript]
tags: [javascript]
description: Javascript te var ve let değişken tanımlamalarındaki farkı nedir.
---


Kısaca şöyle ifade edelim
**var** ile değişken tanımlarsak fonksiyon içerisinde heryerden bu değişkene ulaşabiliriz.

**let** ile değişken tanımlarsak tanımlama yaptığımız iki süslü paranter arasından bu değişkene ulaşabiliriz.
Yani değişkenimiz if bloğu içersinde **let** ile tanımlanmış ise sadece bu if bloğu içinden ulaşılır ve başka yerde
kullanamayız.

Örnek verecek olursak

{% highlight yaml %}

    function deneme()
    {
        var a=12;
        if(true)
        {
	    console.log(a);
        }
    }

    function deneme()
    {
        var a=12;
        if(true)
        {
	    let b=12;
        }
        console.log(b) //burada hata alırız çünkü let ile tanımlandığı için
                      //sadece tanımalandığı süslü paranterler arası kullanılabilir.
    }

// Display data from the object:
document.getElementById("demo").innerHTML = person.fullName();

{% endhighlight %}


Kolay gelsin.

