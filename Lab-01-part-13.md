# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
 `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ            |
| `null`    | ไม่ได้ | ไม่เป็นการตั้งชื่อตัวแปรที่ถูกต้อง             |
| `_value`  | ใช้ได้ | อนุญาตให้ใช้ underscore (_) ในชื่อตัวแปร  |
| `First-name`| ไม่ได้ | มีตัวอักษรพิเศษ (-) ที่ไม่ได้รับอนุญาตในชื่อตัวแปร |
| `Hello!` |    ไม่ได้ | มีตัวอักษรพิเศษ (!) ที่ไม่ได้รับอนุญาตในชื่อตัวแปร |
| `w*h` |    ไม่ได้    | มีการใช้เครื่องหมาย * ที่ไม่ได้รับอนุญาตในชื่อตัวแปร |
| `time` |   ใช้ได้    | ไม่มีปัญหา     |
| `do` |    ใช้ได้   | ไม่มีปัญหา       |
| `Do` |  ใช้ได้     | ไม่มีปัญหา  |
| `21November`| 	ใช้ได้ | ไม่มีปัญหา   |
| `ladkrabang`| ใช้ได้   | ไม่มีปัญหา |
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
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/0ae2be9a-63df-4159-89ae-c7c4ec73b192)

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
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/8dc1086a-891d-4349-acb4-0c25920b254d)


---ผลการทดลอง `byte`
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/ed92fa36-6af7-46a8-bfc1-a3b44d943b3f)


---ผลการทดลอง `short`
 ![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/7c90f656-b83f-4f77-bda8-107f105eedba)


---ผลการทดลอง `ushort`
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/bd50a29f-7ffb-4e95-8da7-b60d29b1cac2)


---ผลการทดลอง `uint`
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/8dfdc89b-a95a-475f-ad24-9d2dcc403e2b)


 

---ผลการทดลอง `float`
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/a2b7a48f-36ca-47bd-9180-a751f8f9378d)

 

---ผลการทดลอง `double`
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/79bdc1f7-4dc0-45ce-b068-06583f55370d)

 
---ผลการทดลอง `decimal`
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/5ba8a56f-8f3f-4407-8f26-704e22f2e76c)

 
---ผลการทดลอง `long`
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/2291d9f9-4915-4709-9ab8-b54df764ddf0)



---ผลการทดลอง `ulong`
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/33161fd0-b476-4292-a47d-a112ef143af7)



---ผลการทดลอง `bool`
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/7b7e6eef-52d9-48f8-9266-7dae0012a7a4)


---ผลการทดลอง `sbyte`
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/9ba09ce2-7ed1-4c8c-9348-aa88d3c37af1)



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

ครั้งที่ 1
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/734df6a1-8b0a-4da3-8d93-2197d27849bb)

ครั้งที่ 2
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/455e525a-a343-408c-9915-9f8893e16e1c)

ครั้งที่ 3 
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/2598a23a-9c81-4685-b334-6d7218bf2d82)

ครั้งที่ 4
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/5e0aecc5-daf6-4b17-b870-bc6a1479ae41)

ครั้งที่ 5
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/4c89dbc3-47f3-4bfd-b6d2-13ae37c804ab)

ครั้งที่ 6
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/f5fa1e11-3295-43a6-91fb-3f0ec46b598c)

ครั้งที่ 7
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/175a6f7f-7818-44cd-98d6-2f7182a6f7ef)

ครั้งที่ 8
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/566f78d2-4cbf-4f43-b2a4-35ae2141bcd9)

ครั้งที่ 9
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/3664fd4c-9bea-4b9a-9752-c13e0d7214b6)

ครั้งที่10
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/00b9b177-72d8-4c3b-b18f-bbc978603a99)




## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
