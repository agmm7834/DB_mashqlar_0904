Faqat `CREATE TABLE`, `INSERT INTO` va `UPDATE` ga asoslangan 20 ta masala:

### Namuna uchun:
# Products SQL

## Jadval yaratish

```sql
CREATE TABLE products (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    name TEXT NOT NULL,
    company TEXT NOT NULL,
    product_count INTEGER DEFAULT 0,
    price INTEGER
);
```

## Ma'lumot qo'shish

```sql
INSERT INTO products (name, company, product_count, price)
VALUES
    ('iPhone 13', 'Apple', 3, 76000),
    ('iPhone 12', 'Apple', 2, 51000),
    ('Galaxy S21', 'Samsung', 2, 56000),
    ('Galaxy S20', 'Samsung', 1, 41000),
    ('P40 Pro', 'Huawei', 5, 36000);
```

## Ma'lumot yangilash

### Barcha mahsulotlar narxini 3000 ga oshirish

```sql
UPDATE products
SET price = price + 3000;
```

### Samsung nomini yangilash

```sql
UPDATE products
SET company = 'Samsung Inc.'
WHERE company = 'Samsung';
```

## Jadval tuzilmasi

| Ustun | Turi | Izoh |
|-------|------|------|
| id | INTEGER | Primary key, avtomatik |
| name | TEXT | Mahsulot nomi, majburiy |
| company | TEXT | Kompaniya nomi, majburiy |
| product_count | INTEGER | Mahsulot soni, default 0 |
| price | INTEGER | Narxi |

## Natija

| id | name | company | product_count | price |
|----|------|---------|---------------|-------|
| 1 | iPhone 13 | Apple | 3 | 79000 |
| 2 | iPhone 12 | Apple | 2 | 54000 |
| 3 | Galaxy S21 | Samsung Inc. | 2 | 59000 |
| 4 | Galaxy S20 | Samsung Inc. | 1 | 44000 |
| 5 | P40 Pro | Huawei | 5 | 39000 |
---

**1.** `students` jadvali yarating (`id`, `name`, `age`, `grade`). 3 ta o'quvchi qo'shing. Keyin barcha o'quvchilarning `grade` ini 5 ga yangilang.

**2.** `cars` jadvali yarating (`id`, `brand`, `model`, `price`). 4 ta mashina qo'shing. Keyin `Toyota` mashinasining narxini 25000 ga o'zgartiring.

**3.** `employees` jadvali yarating (`id`, `name`, `department`, `salary`). 4 ta xodim qo'shing. Keyin barcha xodimlarning maoshini 500 ga oshiring.

**4.** `books` jadvali yarating (`id`, `title`, `author`, `price`). 5 ta kitob qo'shing. Keyin narxi 10000 dan past kitoblarning narxini 10000 ga yangilang.

**5.** `phones` jadvali yarating (`id`, `brand`, `model`, `price`). 4 ta telefon qo'shing. Keyin `Samsung` telefonlarining narxini 5000 ga oshiring.

**6.** `products` jadvali yarating (`id`, `name`, `stock`, `price`). 5 ta mahsulot qo'shing. Keyin `stock` i 0 bo'lgan mahsulotlarning `stock` ini 10 ga yangilang.

**7.** `teachers` jadvali yarating (`id`, `name`, `subject`, `salary`). 4 ta o'qituvchi qo'shing. Keyin `Matematika` fanini o'qituvchilarning maoshini 200 ga oshiring.

**8.** `movies` jadvali yarating (`id`, `title`, `genre`, `rating`). 5 ta film qo'shing. Keyin `rating` i 5 dan past filmlarning ratingini 6 ga yangilang.

**9.** `cities` jadvali yarating (`id`, `name`, `country`, `population`). 4 ta shahar qo'shing. Keyin `Uzbekistan` shaharlarining aholisini 100000 ga oshiring.

**10.** `restaurants` jadvali yarating (`id`, `name`, `city`, `rating`). 4 ta restoran qo'shing. Keyin `Toshkent` dagi restoranlarning ratingini 1 ga oshiring.

**11.** `games` jadvali yarating (`id`, `title`, `platform`, `price`). 5 ta o'yin qo'shing. Keyin `PC` platformasidagi o'yinlarning narxini 15% ga oshiring.

**12.** `clothes` jadvali yarating (`id`, `type`, `brand`, `price`). 5 ta kiyim qo'shing. Keyin `Adidas` brendining narxini 3000 ga kamaytiring.

**13.** `hospitals` jadvali yarating (`id`, `name`, `city`, `beds`). 4 ta kasalhona qo'shing. Keyin barcha kasalhonadagi `beds` sonini 50 ga oshiring.

**14.** `flights` jadvali yarating (`id`, `from_city`, `to_city`, `price`). 4 ta parvoz qo'shing. Keyin `Toshkent` dan uchuvchi parvozlar narxini 20000 ga oshiring.

**15.** `animals` jadvali yarating (`id`, `name`, `species`, `age`). 5 ta hayvon qo'shing. Keyin yoshi 5 dan katta hayvonlarning yoshini 1 ga oshiring.

**16.** `students` jadvali yarating (`id`, `name`, `city`, `score`). 5 ta o'quvchi qo'shing. Keyin `score` i 60 dan past o'quvchilarning `score` ini 60 ga yangilang.

**17.** `laptops` jadvali yarating (`id`, `brand`, `ram`, `price`). 4 ta laptop qo'shing. Keyin `ram` i 8 bo'lgan laptoplarning narxini 10000 ga oshiring.

**18.** `countries` jadvali yarating (`id`, `name`, `population`, `area`). 5 ta davlat qo'shing. Keyin aholisi 10 milliondan kam davlatlarning aholisini 2 barobarga oshiring.

**19.** `courses` jadvali yarating (`id`, `name`, `duration`, `price`). 5 ta kurs qo'shing. Keyin `duration` i 3 oydan kam kurslarning narxini 5000 ga kamaytiring.

**20.** `shops` jadvali yarating (`id`, `name`, `city`, `revenue`). 4 ta do'kon qo'shing. Keyin `Samarkand` dagi do'konlarning `revenue` ini 50000 ga oshiring.
