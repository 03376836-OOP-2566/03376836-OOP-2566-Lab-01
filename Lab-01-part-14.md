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

![Screenshot 2024-01-27 215906](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/6fa56bbd-0fa8-4252-949e-ed7f5e01b96c)



2. `OR`

![Screenshot 2024-01-27 220108](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/88e4eb46-15e4-424f-a4d7-c3e10d6294cd)



3. `NOT`

![Screenshot 2024-01-27 222547](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/08b49762-a7e2-4bbc-a73c-38e3589e676c)



4. `NAND`

![Screenshot 2024-01-27 221603](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/fc1013f0-d3e0-4821-9259-7852047261b7)



5. `NOR`

![Screenshot 2024-01-27 221730](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/ce57043b-0867-4029-99f2-34c1245ce78f)



6. `Exclusive OR`


![Screenshot 2024-01-27 221940](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/08a2c6f8-da28-4a83-9a45-2ac65fbaa343)





## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
