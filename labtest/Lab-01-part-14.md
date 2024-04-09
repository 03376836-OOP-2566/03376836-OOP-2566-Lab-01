![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/2a3dc2c6-2014-4069-804f-0e50509bcacf)# Lab-01 การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ

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
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/642f303b-f738-421c-99b4-3312fa0d7baf)

2. `OR`
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/c4e37714-0a72-4ec8-929a-a0159f0ac7d0)

3. `NOT`
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/e8161c62-6554-4ba0-9264-48b967d7716e)

4. `NAND`
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/9951cf4b-96a5-45bf-a398-3a4c3b9f4184)

5. `NOR`
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/2e1074f1-c6b3-40d2-bdec-556f29af3cf6)

6. `Exclusive OR`
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/67d820e9-00ea-4ebb-a1df-9083c3740449)

## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
