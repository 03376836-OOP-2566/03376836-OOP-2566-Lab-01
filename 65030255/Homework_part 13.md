# 65030255 สรวิชญ์ ชวนเชย
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

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/d44539a3-e924-4903-b5f0-356ad124bec4)

---ผลการทดลอง `byte`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/3cc9f230-67db-4816-9b6a-918c555b1ab5)

---ผลการทดลอง `short`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/85eda727-5dcc-4789-868c-2e092a383b82)

---ผลการทดลอง `ushort`

 ![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/9106d323-fe5b-4831-9bf0-de11c2ef2905)

---ผลการทดลอง `uint`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/fa83163f-ebfa-4d66-9e7a-5ccc5924cdaf)

---ผลการทดลอง `float`
 
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/b518585f-354b-41a8-99c0-0cc013ac3263)

---ผลการทดลอง `double`

 ![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/022d07e8-b55c-4bc4-934c-8ba31e26632e)

---ผลการทดลอง `decimal`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/95a283b4-2483-4eea-84c9-25d7647e5906)
 
---ผลการทดลอง `long`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/a7e00fcb-fb52-4541-a833-a3aa232cd17f)

---ผลการทดลอง `ulong`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/70408dee-5d39-4cfd-b5c2-85594404f3c8)

---ผลการทดลอง `bool`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/0632a8ab-6158-4e39-ba57-39596f0eb6b6)

---ผลการทดลอง `sbyte`

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/43e4efab-0a1f-45fd-bcc2-46f125270e27)

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

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/de914946-c817-40ab-96c9-15d117762ad0)
