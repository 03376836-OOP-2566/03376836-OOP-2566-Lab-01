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
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/d47caffd-4011-4688-8857-e5e8a8b39322)

 
❔ การกำหนดความกว้างของอาร์กิวเมนต์ด้วยเครื่องหมาย { , } ในคำสั่ง ``Console.WriteLine()`` มีรูปแบบการใช้งานอย่างไร
```
การกำหนดความกว้างของอาร์กิวเมนต์ใน Console.WriteLine() ใน C# สามารถทำได้โดยใช้เครื่องหมาย { , } ภายใน string format specifier 
```
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
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/eae495be-5917-4437-be10-6000a8d15801)

❔  การกำหนดตัวอักษร E, F, G, N, P, X หมายถึงให้พิมพ์ออกมาเป็นอะไร
```
การกำหนดตัวอักษรใน string format specifier ใน C# มีผลต่อรูปแบบการแสดงผลของข้อมูล. ตราบใดที่ใช้ตัวอักษรที่แตกต่างกัน, ผลลัพธ์ที่ได้จะมีลักษณะที่แตกต่างกันตามลักษณะของตัวอักษรดังนี้:

{0, 0:E}: แสดงเลขทั้งหมดในรูปแบบที่วิทยาศาสตร์ (Scientific notation).
{0, 0:F}: แสดงเลขทั้งหมดในรูปแบบทศนิยม (Fixed-point notation).
{0, 0:G}: ใช้รูปแบบที่ดีที่สุดระหว่าง Scientific notation และ Fixed-point notation.
{0, 0:N}: แสดงเลขทั้งหมดในรูปแบบทศนิยมพร้อม comma separator สำหรับหลักพัน.
{0, 0:P}: แสดงเลขทั้งหมดในรูปแบบของเปอร์เซ็นต์.
{0, 0:X}: แสดงเลขทั้งหมดในรูปแบบฐาน 16 (Hexadecimal).

``` 

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
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/d74e43c4-ce50-40c5-8615-771e7d0576c5)

## [Part 8  การกำหนดรูปแบบพร้อมความกว้างของทศนิยมของอาร์กิวเมนต์](./Lab-01-part-8.md)
