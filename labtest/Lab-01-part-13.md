![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/81906982-b543-48a6-806a-2d44fc2339bd)# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null` | | |
| `_value` | | |
| `First-name`| | |
| `Hello!` | | |
| `w*h` | | |
| `time` | | |
| `do` | | |
| `Do` | | |
| `21November`| | |
| `ladkrabang`| | |
| `Student ID`| | |


---ผลการทดลอง
ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null` |	ไม่ได้ | null เป็นคีย์เวิร์ดที่ใช้ในภาษา C# เพื่อระบุว่าตัวแปรไม่มีค่าหรือไม่ได้กำหนดค่า |
| `_value` | ใช้ได้ | ตัวแปรสามารถขึ้นต้นด้วย underscore _ ได้ |
| `First-name`|	ไม่ได้ | ไม่สามารถใช้ตัวอักษรขีด (-) ในชื่อตัวแปร |
| `Hello!` |ไม่ได้ | ไม่สามารถใช้เครื่องหมายตัวพิเศษ (!) ในชื่อตัวแปร |
| `w*h` |	ไม่ได้ | ไม่สามารถใช้เครื่องหมายดอกจัน (*) ในชื่อตัวแปร |
| `time` |ใช้ได้ | ไม่มีปัญหา |
| `do` |	ไม่ได้ |	do เป็นคีย์เวิร์ดที่ใช้ใน C# และไม่สามารถใช้เป็นชื่อตัวแปร |
| `Do` | ใช้ได้|	ไม่มีปัญหา |
| `21November`| ใช้ได้| ตัวแปรสามารถขึ้นต้นด้วยตัวเลข |
| `ladkrabang`| ใช้ได้ | ไม่มีปัญหา |
| `Student ID`|	ไม่ได้ | ไม่สามารถใช้เครื่องหมายวรรคตอน (space) ในชื่อตัวแปร |

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
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/38abe3f0-5d27-4bb5-934c-0d3fb48df70a)

---ผลการทดลอง `byte`
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/e86ee506-f621-4eeb-8ac3-0c8afeeffacd)

---ผลการทดลอง `short`
 ![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/4b978bc6-ea52-4d83-ac6d-468d02cc3794)

---ผลการทดลอง `ushort`
 ![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/c7052908-5660-48f7-83e3-5b56162c9b3c)

---ผลการทดลอง `uint`
 ![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/e7bdf4fe-0c8c-4198-a9c5-212a57fe73b1)
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/739922c0-7e66-4e82-9bad-cd1ce28a0642)


---ผลการทดลอง `float`
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/67b8ab4d-90ac-4baf-bb9e-95453df45326)

---ผลการทดลอง `double`
 ![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/61c71f20-9f45-44b2-a065-8b1fada46aa0)

---ผลการทดลอง `decimal`
 ![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/dc1182ae-43d1-432d-af98-728779bee49c)

---ผลการทดลอง `long`

![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/4e0c842f-b2a0-44ff-b196-928dd5584d17)

---ผลการทดลอง `ulong`
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/77e932ef-3e8a-4c34-a517-286ccc432ad8)

---ผลการทดลอง `sbyte`
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/6d2cf1b5-e285-4766-8869-fbaa6c3a7b10)


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
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/ce406f94-fa01-4b81-a67f-89ac62a3ad48)
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/47495043-6de2-4d6f-ae97-4a566740ebed)
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/a5d9487a-92a2-4829-b9f4-20675e7335af)
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/04032371-9eae-4097-a28b-dc751cc9256d)
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/25baac0e-dc5e-4914-b131-99ec44f1172e)
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/249e4086-9907-4a1a-872b-4087a9511afc)
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/b0d33071-0c82-46cc-baca-63c45af49a70)
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/cac843d5-1382-4627-a524-de260f352725)
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/9a45a5e4-98d9-43a7-b26a-579e3aaaf9e4)
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/8df4bd75-8cb4-44b8-b686-0a9333b2cef0)
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/fd4c7cc8-d79a-41d2-bec6-10c2d60a4c37)


## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
