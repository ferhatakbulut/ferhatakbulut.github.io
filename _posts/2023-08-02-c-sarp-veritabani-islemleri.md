---
layout: post
title: json return null problemi
categories: [Genel,Çözüm,C#,Mysql,Veritabanı]
tags: [ipucu,c#,mysql,veritabanı]
fullview: true
---

C# projemizde veritabı bağlantısı için aşağıdaki kod yapısını kullanabilirsiniz.
Bu kod dizimizle vertabanına bağlanbiliriz ve sql komutlarını çalıştarabiliriz artık.

.

Örnek Kod Yapısı

{% highlight yaml %}

    using MySql.Data.MySqlClient;
    // ...

    string connectionString = "server=veritabani_adresi;user=kullanici_adi;password=parola;database=veritabani_adi;";

    using (MySqlConnection connection = new MySqlConnection(connectionString))
    {
        connection.Open();

        string query = "SELECT * FROM tablo_adi";
        using (MySqlCommand command = new MySqlCommand(query, connection))
        {
            using (MySqlDataReader reader = command.ExecuteReader())
            {
                while (reader.Read())
                {
                // Verileri okuyun
                    string veri = reader.GetString(0);
                // ...
                }
            }
        }
    }

{% endhighlight %}



Kolay gelsin.

