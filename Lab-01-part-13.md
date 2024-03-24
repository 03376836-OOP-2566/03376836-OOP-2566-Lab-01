# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null`    | ไม่ได้ | ตั้งชื่อตัวแปรไม่ถูกต้อง  |
| `_value`  | ใช้ได้ |    ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ   |
| `First-name`| ไม่ได้ | มีตัวอักษรพิเศษที่ไม่สามารถตั้งชื่อได้ |
| `Hello!` |  ไม่ได้ | มีตัวอักษรพิเศษที่ไม่สามารถตั้งชื่อได้ |
| `w*h` |  ไม่ได้   |มีตัวอักษรพิเศษที่ไม่สามารถตั้งชื่อได้ |
| `time` |  ใช้ได้  | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ     |
| `do` |   ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ        |
| `Do` |  ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ  |
| `21November`| ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ    |
| `ladkrabang`| ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ  |
| `Student ID`| ไม่ได้   | มีช่องว่างในกฏไม่สามารถตั้งชื่อได้ |


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
![ข้อ 13 char](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/d8392a4f-d23f-4048-aa09-7180255b5a9e)

---ผลการทดลอง `byte`
![ข้อ 13 byte](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/53755142-cd35-413e-9889-dab1ffa7dd7e)

---ผลการทดลอง `short`
 ![ข้อ 13 short](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/7803aa37-801f-435a-83b9-ab50fb7f9dc5)

---ผลการทดลอง `ushort`
![ข้อ 13 ushort](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/653ab019-71e0-4250-b58a-79770e04cfcf)

 ---ผลการทดลอง `uint`
![ข้อ 13 uint](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/3865902d-4a98-4d79-ab5e-abd68a43d048)

 ---ผลการทดลอง `float`
 ![ข้อ 13 float](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/0a688a92-b71f-439e-a979-eb3cb9725897)

---ผลการทดลอง `double`
 ![ข้อ 13 double](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/05c708e1-9119-415e-a487-4b43eda18e10)

---ผลการทดลอง `decimal`
 ![ข้อ 13 decimal](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/15320024-1ee9-49bd-bf8e-99121b9e0160)

---ผลการทดลอง `long`
![ข้อ 13 long](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/6f988cd4-ded2-4ea9-8271-cfac5a53258a)

---ผลการทดลอง `ulong`
![ข้อ 13 ulong](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/06d4fd04-6fb3-407d-ba0a-ab684f05f965)

---ผลการทดลอง `bool`
![ข้อ 13 bool](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/d5d3e841-14c9-45b8-99cc-b1835cf2a4c1)

---ผลการทดลอง `sbyte`
![ข้อ 13 sbyte](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/cdf5c5cc-920a-42d2-baa0-04b0ad739b25)


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

![สุ่ม4](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/db9c10eb-611d-4aa7-a502-62bae86c5756)
![สุ่ม11](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/635650fd-fba7-436a-9d3e-707f9c03e27d)
![สุ่ม12](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/56993294-4949-4153-a769-e09b6b3906c5)
![สุ่ม26](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/05de89a6-7944-4bfa-a98e-75e60fe8c8a3)
![สุ่ม35](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/11c70316-6b82-40b1-92f5-8184d70b1e2a)
![สุ่ม40](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/b829961d-d731-4528-92c2-099983386b4c)
![สุ่ม64](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/0820c09b-0842-4b33-a544-ea3676a4311f)
![สุ่ม68](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/e6e93d38-693b-408c-946a-b1feda404973)
![สุ่ม72](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/6df450f0-2647-4add-9b98-112258d24110)
![สุ่ม88](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/419752bc-3644-4b3f-adcb-bd74f655d1d0)

## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
