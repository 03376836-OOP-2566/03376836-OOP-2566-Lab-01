# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null` | ใช้ไม่ได้ | มีคำสั่งที่ซ้อนกับnull |
| `_value` | ใช้ได้ | ถูกตามหลักสร้างตัวแปร |
| `First-name`| ใช้ไม่ได้ | มีเครื่องหมายทางคณิตศาสตร์ |
| `Hello!` | ใช้ไม่ได้ | มีเครื่องหมายตกใจ |
| `w*h` | ใช้ไม่ได้ | มีเครื่องหมายทางคณิตศาสตร์ |
| `time` | ใช้ได้ | ถูกตามหลักสร้างตัวแปร |
| `do` | ใช้ไม่ได้ | มีคำสั่งที่ซ้อนกับdo |
| `Do` | ใช้ได้ | ถูกตามหลักสร้างตัวแปร |
| `21November`| ใช้ไม่ได้ | ตัวเลขนำหน้าไม่ได้ |
| `Do` | ใช้ได้ | ถูกตามหลักสร้างตัวแปร|
| `ladkrabang`| ใช้ได้ | ถูกตามหลักสร้างตัวแปร |
| `Student ID`| ใช้ไม่ได้ | มีการเว้นว่าง |


---ผลการทดลอง
![12 2](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/872f85c1-8d28-4ab3-a705-efc11f1b8527)


## ชนิดข้อมูลภายในภาษา C\#

Property ของชนิดข้อมูล ในภาษา C# มีชนิดข้อมูลต่างๆ ได้แก่ `byte`, `char`, `bool`, `sbyte`, `short`, `ushort`, `int` , `uint`, `float`, `double`, `decimal`, `long`, `ulong` โดยแต่ละชนิด มีคุณสมบัติที่สำคัญได้แก่ ขนาด (เป็นไบต์) ค่าต่ำสุด ค่าสูงสุด ที่เก็บในตัวแปรชนิดนั้นๆ ได้ ซึ่งมีฟังก์ชันในภาษา C# ที่ช่วยให้เราทราบคุณสมบัติเหล่านั้น ได้แก่คำสั่ง `sizeof()`, `MinValue()` และ `MaxValue()` การแสดงค่าคุณสมบัติต่างๆ ของตัวแปร สามารถทำได้โดยใช้ฟังก์ชั่นเหล่านั้น ดังตัวอย่าง

## 13. โปรแกรมแสดงคุณสมบัติ size, MinValue และ MaxValue ของชนิดข้อมูล

```csharp
Console.WriteLine("Data type : int");
Console.WriteLine("Size :" + sizeof(int));
Console.WriteLine("Minimum Value :" + int.MinValue);
Console.WriteLine("Maximum Value :" + int.MaxValue);
```

### ผลที่ได้จากโปรแกรม

```text
Data type : int
Size :4
Minimum Value :-2147483648
Maximum Value :2147483647
```

👉 คำสั่งสำหรับการทดลอง  

ให้นักศึกษา เขียนโปรแกรมคล้ายกับตัวอย่างในข้อ 13 โดยมีชนิดข้อมูลเป็น `byte`, `char`, `bool`, `sbyte`, `short`, `ushort`, `uint`, `float`, `double`, `decimal`, `long` `และ ulong`  

### หมายเหตุ

ชนิดข้อมูล bool เก็บข้อมูลได้เฉพาะ true และ false ไม่ต้องหา MinValue และ MaxValue

ชนิดข้อมูล char จะต้องมีการ cast ค่า MinValue และ MaxValue ไปยัง int ก่อน ดังนี้

```csharp
Console.WriteLine("Minimum Value :" + (int) char.MinValue);
Console.WriteLine("Maximum Value :" + (int) char.MaxValue);
```
---ผลการทดลอง `char`
![char](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/99475e23-a6d0-457f-b3ba-d9a84b476bac)

---ผลการทดลอง `byte`
![byte](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/71bff0bf-1dd2-47ac-b333-b6366d61b966)

---ผลการทดลอง `short`
![short](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/2412a3fb-f7df-4933-994f-c7e4b64d29d4)


---ผลการทดลอง `ushort`
![ushort](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/71fb33c5-6b1b-4b1b-a363-d143bae119aa)

 

---ผลการทดลอง `uint`
![uint](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/70d5189e-61a2-46b3-a9f1-acd981fb5e6b)

 

---ผลการทดลอง `float`
 
![float](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/f9a6434b-c714-4ec4-a2c5-9beed7a69a4a)

---ผลการทดลอง `double`
![double](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/3a87c880-3692-42fa-99ce-9ede3c40f0ea)

---ผลการทดลอง `decimal`
![decimal](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/0f6bb7bf-8fc6-4aab-852a-f7baeb16bae6)

---ผลการทดลอง `long`
![long](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/a8f58e1b-3ba8-4b08-b49e-c50194676b90)


---ผลการทดลอง `ulong`
![ulong](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/96dabdfd-7332-4c9a-9350-0255f6ac66b2)

---ผลการทดลอง `bool`

---ผลการทดลอง `sbyte`
![sbyte](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/c18486ed-d7f3-4c8e-a1a5-d21246b39c15)

## การใช้งานข้อมูลชนิดต่างๆ

ข้อมูลชนิดตรรกะ The Boolean Type
ข้อมูลชนิดตรรกะ (boolean) มีค่าที่เป็นไปได้เพียง 2 ค่าเท่านั้นคือ true และ false ในภาษา C# จะไม่สามารถกำหนดค่าตัวเลขลงไปในตัวแปร boolean ได้ ส่วนใหญ่ตัวแปร boolean มักใช้เพื่อการตัดสินใจและมีที่มาจากการประเมินค่าสมการต่างๆ ตัวอย่างต่อไปนี้เป็นการใช้ตัวแปร boolean กับการเปรียบเทียบด้วยตัวดำเนินการ “>”
ตัวอย่าง

```csharp
bool a = 4 > 5;
Console.WriteLine("4 > 5 is {0}", a);
```

## สนุกกับการสร้างตัวเลขสุ่ม

ในภาษา C# มีวิธีการสร้างตัวเลขสุ่ม (random number) โดยใช้คลาส Random มาสร้างเป็นตัวแปรโดยมีรูปแบบดังนี้

```csharp
Random random = new Random();
```

เมื่อสร้างแล้ว เราสามารถนำมาหาค่าตัวเลขสุ่มจากตัวแปรดังกล่าว ซึ่งมักจะกำหนดค่าสูงสุดและต่ำสุดในการสุ่มลงไปด้วย ดังนี้

```csharp
int randomNumber = random.Next(0, 100);
```

โปรแกรมด้านล่างนี้เป็นตัวอย่างการสุ่มเลข 0 – 100

```csharp
Random random = new Random();
int randomNumber = random.Next(0, 100);
Console.WriteLine(randomNumber);
```
 
ให้รัน 10 ครั้งแล้วบันทึกค่าที่ได้จากการรัน

## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
