# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null` | ไม่ได้ |ใช้ระบุค่าตัวแปรที่ไม่ได้มีการกำหนดค่าให้ |
| `_value` | ใช้ได้ | ไม่มีปัญหา |
| `First-name`| ไม่ได้ | มีอักขระพิเศษ - |
| `Hello!` | ไม่ได้ | มีอักขระพิเศษ ! |
| `w*h` | ใช้ได้ | ไม่มีปัญหา |
| `time` | ใช้ได้ | ไม่มีปัญหา |
| `do` | ใช้ได้ | ไม่มีปัญหา |
| `Do` | ใช้ได้ | ไม่มีปัญหา|
| `21November`| ใช้ได้ | ไม่มีปัญหา |
| `ladkrabang`| ใช้ได้ | ไม่มีปัญหา |
| `Student ID`| ใช้ได้ | ไม่มีปัญหา |


---ผลการทดลอง
- การตั้งชื่อควรตั้งตามกฎการตั้งชื่อและหลีกเลี่ยงใช้คำที่เป็นkeywordและอักขระพิเศษ

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
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/bbd853b7-be14-4319-918c-3cc37d338b27)

---ผลการทดลอง `byte`
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/14e04eeb-46d8-4247-a28a-28c969359b0c)

---ผลการทดลอง `short`
 ![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/e4a52c55-5136-45ac-8ef0-c1fed884e168)

---ผลการทดลอง `ushort`
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/2d9498b8-417f-4c1a-9f47-4cc9f99973cb)


---ผลการทดลอง `uint`
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/ff82e425-e708-4450-9818-fbd60d979628)

 
---ผลการทดลอง `float`
 ![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/01683a28-b030-403f-88dd-e3412c74d77d)


---ผลการทดลอง `double`
 ![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/71dd8ebd-c7ac-4b4e-b1cd-f0490753ffc2)

---ผลการทดลอง `decimal`
 ![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/7825525a-3e78-4356-b0d5-1f9920bb677a)

---ผลการทดลอง `long`
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/184c4aab-a0e2-4eee-ad2c-963147aa3b4e)


---ผลการทดลอง `ulong`
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/56d58630-89e4-4ebf-8ae4-7246a321e1f6)


---ผลการทดลอง `bool`
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/b495b669-502f-4319-a1d5-8ed9a9f85ab8)


---ผลการทดลอง `sbyte`
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/a0cf52c4-4bdd-4168-8ddc-aaf81f81d7a9)


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
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/dc298575-6698-45d6-873b-99e581060da2)
- ค่าที่ได้ 23 12 39 99 87 68 70 94 56 36
## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
