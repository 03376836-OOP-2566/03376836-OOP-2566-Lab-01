# Lab-01 การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ

ตัวแปรชนิด boolean มักจะถูกใช้เป็นที่เก็บผลที่เกิดจากการดำเนินการทางตรรกะ เช่น AND, OR, NOT เป็นต้น ซึ่งการดำเนินการทางตรรกะจะมีตารางความจริง เป็นตัวบอกผลในการดำเนินการของตัวดำเนินการต่างๆ ดังตัวย่าง

### ตัวดำเนินการ AND

Y = A AND B

| A | B | Y |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

### ตัวดำเนินการ OR

Y = A OR B

| A | B | Y |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

### ตัวดำเนินการ NOT

Y = NOT A

| A | Y |
|--|--|
| 0 | 1 |
| 1 | 0 |

ตัวดำเนินการในภาษา C#
ใช้เครื่องหมายต่างๆ ดังต่อไปนี้

| การดำเนินการ | เครื่องหมาย |
|------------|-----------|
| Logical AND | & |
| Logical XOR | ^ |
| Logical OR | \| |

## 14. การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ

ตัวอย่างภาษา C# ต่อไปนี้เป็นการพิมพ์ตารางความจริงออกทางหน้าจอ
👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
bool A, B,Y;
Console.WriteLine("      Y = A AND B");
Console.WriteLine("-----------------------");
Console.WriteLine("   A      B\t|  Y");
Console.WriteLine("-----------------------");
A = false; B = false; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A,B,Y);
A = false; B = true; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
A = true; B = false; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
A = true; B = true; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
Console.WriteLine("-----------------------");
```

➢ รันโปรแกรมและบันทึกผล
![ข้อ 14 1](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/7b51e560-feb1-4229-b2f6-1fe434b47c87)

 
👷 จากข้อ 14 ให้เขียนโปรแกรมเพื่อสร้างตารางความจริงของลอจิกดังต่อไปนี้

## โค้ดการทำงานของโปรแกรมในข้อที่ 14
![โค้ดข้อ14 1](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/d26f39c1-5619-41db-a3cf-b26d503dbb3b)
![โค้ดข้อ14 2](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/a1e03eb2-0a5b-40fe-a458-4fbc74c071f2)

1. `AND`

![ข้อ 14 2 1](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/2ef235db-32f7-4d14-8fc9-35e0e3751a38)

2. `OR`

![ข้อ 14 2 2](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/6b487a1c-51dd-4033-a250-7568486a1dfa)

3. `NOT`

![ข้อ 14 2 3](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/9b309964-5413-4130-bcd6-b157e0339754)

4. `NAND`

![ข้อ 14 2 4](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/5187e197-3f3f-4f09-87cc-efaa6bbaeaaa)

5. `NOR`

![ข้อ 14 2 5](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/e5960a62-cdad-49c6-86a0-9ab37227065c)

6. `Exclusive OR`

![ข้อ 14 2 6](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/22aaf434-0ad8-4b7a-aaa9-6311901a82ad)


## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
