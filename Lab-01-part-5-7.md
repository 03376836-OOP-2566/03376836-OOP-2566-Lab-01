# Lab-01 Part 5 การกำหนดความกว้างของอาร์กิวเมนต์

เราสามารถแกหนดตำแหน่งของอักขระที่จะพิม์ออกทาง output ได้ โดยการใช้รูปแบบ { i, j }
โดย i ยังคงเป็นลำดับที่ตามตำแหน่งของ place holder และ j คือจำนวนช่องว่างทีต้องการ

👉แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
Console.WriteLine("00000000011111111112");
Console.WriteLine("12345678901234567890");
Console.WriteLine("{0, 0}", 1);
Console.WriteLine("{0, 1}", 1);
Console.WriteLine("{0, 2}", 1);
Console.WriteLine("{0, 3}", 1);
Console.WriteLine("{0, 5}", 1);
Console.WriteLine("{0, 10}", 1);
Console.WriteLine("{0, 15}", 1);
Console.WriteLine("{0, 20}", 1);
```

หมายเหตุ ตัวเลขสองบรรทัดบนสุด ใช้เพื่อกำหนดตำแหน่ง column ของตัวอักษร

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/52b5fe79-5640-4d57-951c-eb95674da741)
 
❔ การกำหนดความกว้างของอาร์กิวเมนต์ด้วยเครื่องหมาย { , } ในคำสั่ง ``Console.WriteLine()`` มีรูปแบบการใช้งานอย่างไร

### คือ Console.WriteLine("{index[,width]}", arg1, arg2, ...); โดย index = ตำแหน่ง index ที่จะถูกใช้แทนค่าข้อมูล width = ตำแหน่งของข้อมูลที่จะแสดงผลออกมาทางจอ

## 6. การกำหนดรูปแบบของอาร์กิวเมนต์

👉 แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
int n = 123456789;
Console.WriteLine("{0, 0:E}", n);
Console.WriteLine("{0, 0:F}", n);
Console.WriteLine("{0, 0:G}", n);
Console.WriteLine("{0, 0:N}", n);
Console.WriteLine("{0, 0:P}", n);
Console.WriteLine("{0, 0:X}", n);
```

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/6d8f7730-7fc9-42a2-a612-f4f1a3ab7060)

❔  การกำหนดตัวอักษร E, F, G, N, P, X หมายถึงให้พิมพ์ออกมาเป็นอะไร

### {0, 0:E}: แสดงเป็นตัวเลขทางวิทยาศาสตร์ (Scientific Notation)
### {0, 0:F}: แสดงเป็นทศนิยม
### {0, 0:G}: แสดงเป็นรูปแบบที่ดีที่สุดตามเงื่อนไขที่กำหนด (General Format)
### {0, 0:N}: แสดงเป็นจำนวนเต็มที่มีการคั่นหลักทุก 3 ตำแหน่ง
### {0, 0:P}: แสดงเป็นร้อยละ(%)
### {0, 0:X}: แสดงเป็นเลขฐาน 16 (Hexadecimal)

## 7. การกำหนดรูปแบบพร้อมความกว้างของอาร์กิวเมนต์

👉 แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
int n = 123456789;
Console.WriteLine("{0, 20:E}", 1);
Console.WriteLine("{0, 20:F}", 1);
Console.WriteLine("{0, 20:G}", 1);
Console.WriteLine("{0, 20:N}", 1);
Console.WriteLine("{0, 20:P}", 1);
Console.WriteLine("{0, 20:X}", 1);
```

➢   รันโปรแกรมและบันทึกผล

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/f1f72992-0ff3-4e5a-81c9-ac21c468b96a)
 
## [Part 8  การกำหนดรูปแบบพร้อมความกว้างของทศนิยมของอาร์กิวเมนต์](./Lab-01-part-8.md)
