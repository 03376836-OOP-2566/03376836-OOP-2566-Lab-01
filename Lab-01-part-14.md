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
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/79557d7f-ef46-4824-b9a5-4c5d631269bd)

 
👷 จากจ้อ 14 ให้เขียนโปรแกรมเพื่อสร้างตารางความจริงของลอจิกดังต่อไปนี้

1. `AND`
   ![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/79557d7f-ef46-4824-b9a5-4c5d631269bd)
2. `OR`
 ![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/0c6c5ff2-3e14-46cb-9de4-c3f77cdf5098)


3. `NOT`
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/f07e5874-8266-405c-b572-8f0e780aea52)
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/b422fc6c-1d39-4238-bdf2-c036ca615418)

4. `NAND`
 ![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/0b9b4811-17b8-41f9-aca5-986210bfe9db)

5. `NOR`
 ![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/b8e94464-001d-4da1-a5f7-c4f5e5eb4658)

6. `Exclusive OR `
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/e4559f8b-45f1-4f87-a8b9-589c314245ac)


## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
