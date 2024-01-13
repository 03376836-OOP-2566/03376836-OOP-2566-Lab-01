# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ            |
| `null`    | ไม่ได้ | ไม่เป็นการตั้งชื่อตัวแปรที่ถูกต้อง             |
| `_value`  | ใช้ได้ |    ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ   |
| `First-name`| ไม่ได้ | มีตัวอักษรพิเศษ (-) ที่ไม่ได้รับอนุญาตในชื่อตัวแปร |
| `Hello!` |  ไม่ได้ | มีตัวอักษรพิเศษ (!) ที่ไม่ได้รับอนุญาตในชื่อตัวแปร |
| `w*h` |  ไม่ได้   | มีการใช้เครื่องหมาย * ที่ไม่ได้รับอนุญาตในชื่อตัวแปร |
| `time` |  ใช้ได้  | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ     |
| `do` |   ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ        |
| `Do` |  ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ  |
| `21November`| ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ    |
| `ladkrabang`| ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ  |
| `Student ID`| ไม่ได้   | มีช่องว่างที่ไม่ได้รับอนุญาตในชื่อตัวแปร |


---ผลการทดลอง


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

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/0ee36ccf-0952-4840-a626-9b9c05d8fa02)

---ผลการทดลอง `byte`

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/86ccd7f1-9ce1-4d56-a675-80d459d69773)

---ผลการทดลอง `short`
 
![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/ed25f801-10c2-426b-a329-5579ef3d0077)

---ผลการทดลอง `ushort`

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/3c3ee3a7-c0fc-454b-a2b2-744133e899e1)

---ผลการทดลอง `uint`

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/2dabb44b-2faa-4bea-94fb-3319c1cfa7ed)
 
---ผลการทดลอง `float`
 
![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/e6d2fbc4-7ea4-40be-84aa-dc1bf183687e)

---ผลการทดลอง `double`

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/91f49227-23f2-4337-b647-9ff46334831f)

---ผลการทดลอง `decimal`

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/9009cb3c-9fc4-492c-8c07-5cb39c583114)
 
---ผลการทดลอง `long`

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/7fb8139a-ac9a-4413-8335-b3fee0458947)

---ผลการทดลอง `ulong`

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/91503b28-94d1-48ce-85fe-7462dcbeebb7)

---ผลการทดลอง `bool`

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/c62a04f8-4962-42f7-9db6-8ae7494535aa)

---ผลการทดลอง `sbyte`

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/8ed14fec-ca4a-4a44-baf3-6897898f522d)

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

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/45e6a289-f8b8-469f-979a-8bba3e36e662)

## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
