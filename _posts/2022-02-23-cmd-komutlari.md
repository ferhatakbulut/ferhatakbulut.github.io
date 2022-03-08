---
layout: post
title: Bazı Cmd Komutları
categories: [windows, cmd]
tags: [cmd, komutlar]
description: Bazı Cmd Komutları ve Açıklamaları
---


<table border='1'>
	<tr>
	<th>Komut</th>
	<th></th>
	<th>Açıklama</th>
	</tr>
	<tr>
	<td>shutdown /r /m \\192.168.1.22</td>
	<td>:</td>
	<td>İlgli ip deki bilgisayarı uzaktan yeniden başlat</td>
	</tr>
	<tr>
	<td>shutdown /s /m \\192.168.1.22</td>
	<td>:</td>
	<td>İlgli ip deki bilgisayarı uzaktan kapat</td>
	</tr>

	<tr>
	<td>shutdown /s /m  \\192.168.1.22 /f /c "Selamlar"</td>
	<td>:</td>
	<td>İlgli ip deki bilgisayarı uzaktan kapatır ve ekranda mesaj gösterir</td>
	</tr>

	<tr>
	<td>msg /SERVER:192.168.1.22 * /TIME:60 "selamlar"</td>
	<td>:</td>
	<td>İlgli ip deki bilgisayarı uzaktan mesaj gönderir</td>
	</tr>
</table>


<br>

Çalıştır geçmişini temizleme komutu

{% highlight yaml %}

   reg delete HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\RunMRU /va /f

{% endhighlight %}


Kolay gelsin.

