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
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/be5d8441-02da-42b5-a57e-73b6532c538a)

 
👷 จากจ้อ 14 ให้เขียนโปรแกรมเพื่อสร้างตารางความจริงของลอจิกดังต่อไปนี้

1. `AND`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/be5d8441-02da-42b5-a57e-73b6532c538a)
2. `OR`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/b3c5a97a-c2df-4705-a72b-5d95c5ebd0bc)

3. `NOT`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/4a177842-8064-4104-9bc3-e2413b80f50d)

4. `NAND`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/458517a5-0ab0-4d69-8c85-1ceb61cc4dd5)

5. `NOR`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/ecb4f293-40f3-4766-85c3-7d1216040794)

6. `Exclusive OR`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/a82dd5ab-cc4d-4aa7-bca5-80a643332a02)


## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
