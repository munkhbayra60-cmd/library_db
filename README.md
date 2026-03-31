# 📚 Library Management System (SQL Project)

Энэхүү төсөл нь Номын сангийн мэдээллийн системийн өгөгдлийн санг төлөвлөх, хөгжүүлэх, болон аюулгүй байдлыг хангах даалгаврын хүрээнд хийгдсэн болно.

## 🛠 Ашигласан технологиуд
* **Database:** MySQL / MariaDB
* **Tools:** MySQL Workbench, Command Line (mysqldump)
* **Version Control:** Git & GitHub

## 📂 Төслийн бүтэц
* `mysqlScript.sql`: Өгөгдлийн сан үүсгэх, хүснэгтүүдийн хамаарал, жишээ өгөгдөл болон SQL query-үүд багтсан үндсэн файл.
* `library_db_backup.sql`: Өгөгдлийн сангийн нөөц хуулбар (Backup).

## 🚀 Хэрхэн ажиллуулах вэ?

1. **Өгөгдлийн санг үүсгэх:**
   `mysqlScript.sql` файлыг MySQL программ дээрээ ажиллуулна. Энэ нь автоматаар `library_db` нэртэй database үүсгэж, шаардлагатай хүснэгтүүдийг (members, books, borrow_records, librarians) үүсгэнэ.

2. **Backup-аас сэргээх (Restore):**
   Хэрэв танд backup файл байгаа бол дараах тушаалаар сэргээж болно:
   ```bash
   mysql -u root -p library_db < library_db_backup.sql
