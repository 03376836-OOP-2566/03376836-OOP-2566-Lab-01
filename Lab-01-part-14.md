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

 
👷 จากจ้อ 14 ให้เขียนโปรแกรมเพื่อสร้างตารางความจริงของลอจิกดังต่อไปนี้

1. `AND`
## ![Screenshot 2024-03-23 230259](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/ead24c4a-9f31-48d9-9cce-3a1ccff43426)

2. `OR`
## ![Screenshot 2024-03-23 230322](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/9ea691a8-2386-43a5-9f1d-97b0d276de70)

3. `NOT`
## ![Screenshot 2024-03-23 230344](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/a9c5bdd0-1e82-406e-94e8-6df982b7ae30)

4. `NAND`
## ![Screenshot 2024-03-23 230415](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/7e626822-fbc6-491c-9759-bbb1f080a256)

5. `NOR`
## ![Screenshot 2024-03-23 230434](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/4a05d481-ab31-431a-8636-f785d3611abd)

6. `Exclusive OR`
## ![Screenshot 2024-03-23 230644](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/b4e185cb-61b3-489a-b221-3462ec33386c)


## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
