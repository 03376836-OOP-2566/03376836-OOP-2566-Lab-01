# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null` | ใช้ได้ | null เป็นคีย์เวิร์ดที่ใช้ในการระบุค่าของตัวแปรที่ไม่ได้กำหนดค่า (null) |
| `_value` | ใช้ได้ | ไม่มีปัญหาในการตั้งชื่อ |
| `First-name`| ไม่ได้ | มีการใช้ hyphen (-) ซึ่งไม่ได้รับอนุญาตในการตั้งชื่อตัวแปร |
| `Hello!` | ไม่ได้ | มีใช้ตัวอักษรพิเศษ (!) ที่ไม่ได้รับอนุญาตในการตั้งชื่อตัวแปร |
| `w*h` | ไม่ได้| มีใช้ตัวอักษรพิเศษ (*) ที่ไม่ได้รับอนุญาตในการตั้งชื่อตัวแปร |
| `time` | ใช้ได้ | ไม่มีปัญหาในการตั้งชื่อ |
| `do` | ใช้ได้ | ไม่มีปัญหาในการตั้งชื่อ |
| `Do` | ใช้ได้ | ไม่มีปัญหาในการตั้งชื่อ |
| `21November`|  ใช้ได้ |  ไม่มีปัญหาในการตั้งชื่อ |
| `ladkrabang`| ใช้ได้ | ไม่มีปัญหาในการตั้งชื่อ |
| `Student ID`| ไม่ได้ | มีการใช้ space ที่ไม่ได้รับอนุญาตในการตั้งชื่อตัวแปร |


---ผลการทดลอง
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/a56d8feb-47f9-44b0-8b7f-a1fd4daf634b)


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

![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/2b0b7477-109d-4115-97f0-cba54ad8e177)

ให้นักศึกษา เขียนโปรแกรมคล้ายกับตัวอย่างในข้อ 13 โดยมีชนิดข้อมูลเป็น `byte`, `char`, `bool`, `sbyte`, `short`, `ushort`, `uint`, `float`, `double`, `decimal`, `long` `และ ulong`  
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/9fe79eea-90dd-4041-91b3-1a0c360518e3)

### หมายเหตุ

ชนิดข้อมูล bool เก็บข้อมูลได้เฉพาะ true และ false ไม่ต้องหา MinValue และ MaxValue

ชนิดข้อมูล char จะต้องมีการ cast ค่า MinValue และ MaxValue ไปยัง int ก่อน ดังนี้

```csharp
Console.WriteLine("Minimum Value :" + (int) char.MinValue);
Console.WriteLine("Maximum Value :" + (int) char.MaxValue);
```
---ผลการทดลอง `char`
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/ae0e5a05-d95c-4bf3-aab6-741b24462c06)

---ผลการทดลอง `byte`
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/8a8eedbb-9e8c-4cf6-9364-26ae807671f4)

---ผลการทดลอง `short`
 ![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/3fcba6b7-219b-4875-b1f1-f18de32c4e7f)


---ผลการทดลอง `ushort`
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/f0812bb5-e4b9-4298-bcb8-d701f38df622)



 

---ผลการทดลอง `uint`
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/ceab1985-199b-4d55-88d7-24a586b37b6e)

 

---ผลการทดลอง `float`
 ![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/e1f7521b-37dd-4b98-a2af-70827ecf1da9)


---ผลการทดลอง `double`
 ![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/6ed88a33-f0b8-4405-8718-bfcab3ad6f6e)

---ผลการทดลอง `decimal`
 ![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/dc2f96a9-ba64-4873-a6e9-18171336fefa)

---ผลการทดลอง `long`
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/a99a01ea-8502-4190-8584-5167f64829da)


---ผลการทดลอง `ulong`
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/e56424ab-9033-4ebe-9060-e0e23372df9d)


---ผลการทดลอง `bool`
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/fbebd3f2-6397-49f9-a4b8-898936bacf1b)
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/3f692bef-d6d3-435c-9c54-12db0194658f)


---ผลการทดลอง `sbyte`
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/73f4cd83-b7a3-44a5-95d7-0c67069fdc0e)


## การใช้งานข้อมูลชนิดต่างๆ

ข้อมูลชนิดตรรกะ The Boolean Type
ข้อมูลชนิดตรรกะ (boolean) มีค่าที่เป็นไปได้เพียง 2 ค่าเท่านั้นคือ true และ false ในภาษา C# จะไม่สามารถกำหนดค่าตัวเลขลงไปในตัวแปร boolean ได้ ส่วนใหญ่ตัวแปร boolean มักใช้เพื่อการตัดสินใจและมีที่มาจากการประเมินค่าสมการต่างๆ ตัวอย่างต่อไปนี้เป็นการใช้ตัวแปร boolean กับการเปรียบเทียบด้วยตัวดำเนินการ “>”
ตัวอย่าง

```csharp
bool a = 4 > 5;
Console.WriteLine("4 > 5 is {0}", a);
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/b1194a6a-8eec-4c2d-860c-0f752ba3a604)

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
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/01698dbd-273b-4d19-801f-d89df24e6504)
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/9e2d439c-a8b8-4148-be7d-61787d9026b4)
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/f6fd8dc3-b298-4565-9c49-97539ac842bd)
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/69511201-9cac-4c3e-a3bf-93cafc43dd49)
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/f2472b13-6fbe-487d-a971-01a5e4ff5e9f)
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/59da72db-baac-4d78-b821-cbb8846889db)
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/a79eb626-b974-420d-bbd1-41fa116d5f74)
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/ffe3acc5-310e-4340-9a4e-61ed29b77dbe)
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/7507f01e-4117-4136-9e04-19a7db5827be)
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/bed315eb-6af0-4fda-9877-41122644dfb9)




## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
