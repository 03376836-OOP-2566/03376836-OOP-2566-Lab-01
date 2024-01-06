# 65030255
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

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/e582c3c3-b076-43d0-a6fb-6038b3cd5eaa)

 
👷 จากจ้อ 14 ให้เขียนโปรแกรมเพื่อสร้างตารางความจริงของลอจิกดังต่อไปนี้

1. `AND`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/5affda97-f7d5-43c1-a788-a165450d5399)

2. `OR`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/1530a1bf-4e11-4dcb-a7fa-95bfc5af0cb2)

3. `NOT`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/810f3d9f-d055-4e7b-9da6-e289e7bed275)

4. `NAND`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/ca563eaa-b302-47b0-b3a4-b77924f5bd10)

5. `NOR`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/519652d3-b33e-42a1-bede-5ca7fd229095)

6. `Exclusive OR`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/05712c42-552a-4ab0-b6b4-1c4a13ebcfbd)

## Code

        bool A, B, Y;
        // AND
        Console.WriteLine("      Y = A AND B");
        Console.WriteLine("-----------------------");
        Console.WriteLine("   A      B\t|  Y");
        Console.WriteLine("-----------------------");
        A = false; B = false; Y = A & B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = false; B = true; Y = A & B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = true; B = false; Y = A & B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = true; B = true; Y = A & B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        Console.WriteLine("-----------------------");

        // OR
        Console.WriteLine("\n      Y = A OR B");
        Console.WriteLine("-----------------------");
        Console.WriteLine("   A      B\t|  Y");
        Console.WriteLine("-----------------------");
        A = false; B = false; Y = A | B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = false; B = true; Y = A | B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = true; B = false; Y = A | B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = true; B = true; Y = A | B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        Console.WriteLine("-----------------------");

        // NOT
        Console.WriteLine("\n      Y = NOT A");
        Console.WriteLine("-----------------------");
        Console.WriteLine("   A\t|  Y");
        Console.WriteLine("-----------------------");
        A = false; Y = !A;
        Console.WriteLine(" {0}\t| {1}", A, Y);
        A = true; Y = !A;
        Console.WriteLine(" {0}\t| {1}", A, Y);
        Console.WriteLine("-----------------------");

        // NAND
        Console.WriteLine("\n      Y = A NAND B");
        Console.WriteLine("-----------------------");
        Console.WriteLine("   A      B\t|  Y");
        Console.WriteLine("-----------------------");
        A = false; B = false; Y = !(A & B);
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = false; B = true; Y = !(A & B);
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = true; B = false; Y = !(A & B);
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = true; B = true; Y = !(A & B);
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        Console.WriteLine("-----------------------");

        // NOR
        Console.WriteLine("\n      Y = A NOR B");
        Console.WriteLine("-----------------------");
        Console.WriteLine("   A      B\t|  Y");
        Console.WriteLine("-----------------------");
        A = false; B = false; Y = !(A | B);
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = false; B = true; Y = !(A | B);
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = true; B = false; Y = !(A | B);
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = true; B = true; Y = !(A | B);
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        Console.WriteLine("-----------------------");

        // Exclusive OR (XOR)
        Console.WriteLine("\n      Y = A XOR B");
        Console.WriteLine("-----------------------");
        Console.WriteLine("   A      B\t|  Y");
        Console.WriteLine("-----------------------");
        A = false; B = false; Y = A ^ B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = false; B = true; Y = A ^ B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = true; B = false; Y = A ^ B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        A = true; B = true; Y = A ^ B;
        Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
        Console.WriteLine("-----------------------");
