---
layout: post
title: javascript Yararlı Bilgiler
categories: [Genel,Çözüm,Javascript]
tags: [javascript]
description: Javascript de kullanabileceğiniz yararlı bilgiler.
---

Javascript de kullanabileceğiniz yararlı bilgiler. 

{% highlight yaml %}

    person = {
      firstName: "John",
      lastName: "Doe",
      id: 5566,
      fullName: function() {
        return this.firstName + " " + this.lastName;
      }
  };

// Display data from the object:
document.getElementById("demo").innerHTML = person.fullName();

{% endhighlight %}


Kolay gelsin.

