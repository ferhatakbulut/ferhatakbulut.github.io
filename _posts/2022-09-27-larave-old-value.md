---
layout: post
title: Laravel de post işlemi hatalı dönerken inputlara girilen değerlerin silinmemesi
categories: [Genel,Html,Php,Laravel]
tags: [old,value]
fullview: true
---

Laravel form post işlemi yaparken hatalı bir mesaj döndürüken inputlara girilen verilerin silinmemsi yani forma
girilmiş olan verilerin korunmuş bir şekilde tekrar dönmesi için 

View' de bulunan form elemanı inputlar için aşağıdaki şekilde **value="{{ old('isim') }}"** şeklinde value özelliğini yazıyoruz.

{% highlight yaml %}

    <input name="isim" type="text"  value="{{ old('isim') }}">

{% endhighlight %}

Controller kısmında fonksiyon kısmımızda ise **withInput()** parametresini ekliyoruz. Bu sayede hatalı bir işlem dönse bile formdaki eski
verilerimiz korunmuş bir şekilde formumuz geri dönecektir.

{% highlight yaml %}

    return Redirect::back()->with('hata', 'Telefon Numarası Daha Önceden Var')->withInput();

{% endhighlight %}


Kolay gelsin.

