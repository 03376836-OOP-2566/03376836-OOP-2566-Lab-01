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

1. `AND`<img width="859" alt="Screenshot 2024-03-23 232152" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/9ae86a19-1642-4b33-9288-3de1fe54e6ab">

2. `OR`<img width="866" alt="Screenshot 2024-03-23 232216" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/fa3a2f0f-b642-41a2-b551-2b0eb5ac1f38">

3. `NOT`<img width="858" alt="Screenshot 2024-03-23 232301" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/18480ecb-5ee1-4b0b-8fa3-487c68169f64">

4. `NAND`<img width="859" alt="Screenshot 2024-03-23 232329" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/56f956f4-ed7c-442a-9144-50e78907c5c6">

5. `NOR`<img width="850" alt="Screenshot 2024-03-23 232350" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/9ae0d8ad-7f6f-4089-aace-68fa2b72313e">

6. `Exclusive OR`<img width="852" alt="Screenshot 2024-03-23 232417" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/9defbd01-e506-46e2-8ef5-4c534d6c41fa">



## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
