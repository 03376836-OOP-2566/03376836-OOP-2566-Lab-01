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
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/55e6983c-9944-4a54-9ab0-effe7ed5b574)

 
❔ การกำหนดความกว้างของอาร์กิวเมนต์ด้วยเครื่องหมาย { , } ในคำสั่ง ``Console.WriteLine()`` มีรูปแบบการใช้งานอย่างไร
ตอบ Console.WriteLine("{0:10}".format("Hello"))
1. {0} แทนอาร์กิวเมนต์ตัวแรก
2. :10 ระบุความกว้าง 10 ตัวอักษร
3. ข้อความ "Hello" จะถูกเติมช่องว่างด้านหน้าจนเต็ม 10 ตัวอักษร


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
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/17aead6a-989b-4961-b35d-8e0ff66c2c83)

❔  การกำหนดตัวอักษร E, F, G, N, P, X หมายถึงให้พิมพ์ออกมาเป็นอะไร
ตอบ ตัวอักษร E, F, G, N, P, X ที่ใช้ใน Console.WriteLine("{0, 0:X}", n) หมายถึงรูปแบบการพิมพ์ข้อมูลดังนี้:

1. E: พิมพ์ข้อมูลแบบเลขชี้กำลัง (Scientific notation)

ตัวอย่าง: 123456789 -> 1.234568e+08

2. F: พิมพ์ข้อมูลแบบทศนิยม (Fixed-point notation)

ตัวอย่าง: 123456789 -> 123456789.000000

3. G: พิมพ์ข้อมูลแบบทั่วไป (General format)

ตัวอย่าง: 123456789 -> 1.234568e+08 (เลือกแบบ E หรือ F ขึ้นอยู่กับความยาว)

4. N: พิมพ์ข้อมูลแบบตัวเลข (Number with thousands separator)

ตัวอย่าง: 123456789 -> 123,456,789.00

5. P: พิมพ์ข้อมูลแบบเปอร์เซ็นต์ (Percentage)

ข้อควรระวัง:

รูปแบบ P ไม่รองรับกับ int ใน .NET
6. X: พิมพ์ข้อมูลแบบเลขฐานสิบหก (Hexadecimal)

ตัวอย่าง: 123456789 -> 753B7FFF
 

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
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/b0f7e9a9-d9ae-4a1f-836a-5eb5d61bb523)

 
## [Part 8  การกำหนดรูปแบบพร้อมความกว้างของทศนิยมของอาร์กิวเมนต์](./Lab-01-part-8.md)
