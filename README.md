# PostgreSQL ile Film Kiralama Sistemi Veritabanı Mimarisi

## Genel Bakış
Bu proje, bir film kiralama platformunun arka planındaki karmaşık veri ilişkilerini ve iş mantığını yönetmek amacıyla tasarlanmış ilişkisel bir veritabanı çalışmasıdır. Proje, PostgreSQL üzerinde ORM araçları kullanılmadan, tamamen ham SQL ve veritabanı odaklı bir yaklaşımla (Database-first) geliştirilmiştir.

## Teknik Özellikler
* **İlişkisel Modelleme:** 10'dan fazla tablo, çoktan çoğa (N:M) ilişkiler ve **Inheritance** (Kalıtım) yapısı kullanılarak kurgulanmış mimari.
* **İleri Seviye SQL Yapıları:** Karmaşık iş mantığını (Business Logic) otomatize etmek için geliştirilmiş **Stored Procedures**, **Functions** ve **Triggers**.
* **Veri Bütünlüğü (Data Integrity):** Foreign Key kısıtlamaları, Check Constraints ve tetikleyicilerle sağlanan yüksek seviyeli veri güvenliği.
* **No ORM:** Veritabanı performansını optimize etmek için tüm işlemler doğrudan SQL sorguları ve veritabanı fonksiyonları üzerinden yönetilmiştir.

## Teknoloji Yığını
* **Database:** PostgreSQL
* **Language:** PL/pgSQL
* **Architecture:** Relational Database Design (ERD / Crow's Foot Notation)
* **Approach:** Database-first (No ORM)
