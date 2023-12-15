- Test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
```SQL
CREATE TABLE employee (
	id SERIAL PRIMARY KEY,
	first_name VARCHAR(50) NOT NULL,
	birthday DATE,
	email VARCHAR(100) NOT NULL
);
```
- Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
DONE!
- Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
```SQL
UPDATE employee
SET first_name = 'Tufan'
WHERE id=1;
```
- Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
```SQL
DELETE FROM employee
WHERE first_name = 'Tufan';
```