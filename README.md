# Mini Project SQL: TheLook E-commerce

Proyek portofolio SQL ini dibuat sebagai bagian dari **Data Analytics Bootcamp**. Proyek ini mendemonstrasikan kemampuan dasar hingga menengah dalam menggunakan SQL (Google BigQuery) untuk mengekstrak, menggabungkan, dan menganalisis data dari *TheLook E-commerce* guna menjawab berbagai kebutuhan bisnis.

---

## 🎯 Tujuan Proyek
Berperan sebagai **Junior Data Analyst** di TheLook E-commerce untuk membantu tim bisnis (Product, Marketing, dan CRM) memahami karakteristik produk, perilaku pemesanan pelanggan, serta kategori produk yang memberikan kontribusi terbesar terhadap penjualan melalui analisis berbasis data menggunakan SQL.

---

## 📊 Dataset
Analisis ini menggunakan dataset publik BigQuery:
- **Project/Dataset:** `bigquery-public-data.thelook_ecommerce`
- **Tabel yang Digunakan:**
  1. `products` (Informasi detail produk, kategori, merek, dan harga)
  2. `users` (Informasi demografi dan data pelanggan)
  3. `orders` (Data transaksi pemesanan dan status pesanan)
  4. `order_items` (Detail item per pesanan termasuk harga jual dan status)

---

## 📝 Pertanyaan Bisnis & Implementasi SQL

Berikut adalah 5 pertanyaan bisnis yang diselesaikan menggunakan query SQL:

### 1. Analisis Produk (Karakteristik Dasar)
* **Kebutuhan Tim Product:** Mengetahui karakteristik produk yang dijual di platform.
* **Materi SQL:** `SELECT`, `FROM`, `LIMIT`
* **Query:**
  ```sql
  SELECT 
    name, 
    category, 
    department, 
    brand, 
    retail_price
  FROM 
    `bigquery-public-data.thelook_ecommerce.products`
  LIMIT 20;
