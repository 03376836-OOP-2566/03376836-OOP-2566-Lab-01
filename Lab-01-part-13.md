# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


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
![Screenshot 2024-03-25 011623](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/5be3b75e-6a9a-4957-81a7-5e7272296758)

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
![Screenshot 2024-03-25 011903](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/3fde690d-4f70-4714-8e4d-2f4b44547ece)

---ผลการทดลอง `byte`
![Screenshot 2024-03-25 011738](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/28a9c875-1075-4b26-acf8-d1f7aef7fac8)

---ผลการทดลอง `short`
 ![Screenshot 2024-03-25 012404](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/eee6c732-ff37-4911-a20a-b56356f3c32c)


---ผลการทดลอง `ushort`
![Screenshot 2024-03-25 012440](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/3bbad933-2546-4968-9558-f830bafd544c)

 

---ผลการทดลอง `uint`
![Screenshot 2024-03-25 012518](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/6492dce0-591d-41a9-abf8-790abc1a59f2)

 

---ผลการทดลอง `float`
 ![Screenshot 2024-03-25 012557](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/64fa0652-19f2-4206-9661-a64ebe643e5f)


---ผลการทดลอง `double`
 ![Screenshot 2024-03-25 012633](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/42db2508-438a-430a-a3e0-1499ab2cd337)

---ผลการทดลอง `decimal`
 ![Screenshot 2024-03-25 012712](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/6027342a-040d-4cb2-a1e6-b8fa20a21fdf)

---ผลการทดลอง `long`
![Screenshot 2024-03-25 012747](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/d494dc28-07b9-44f9-8ec2-4608df7ffdf7)


---ผลการทดลอง `ulong`
![Screenshot 2024-03-25 012814](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/45e58fed-7de6-4a8f-99cd-5fedf89d0f99)


---ผลการทดลอง `bool`
![Screenshot 2024-03-25 012226](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/7f9adfdc-513a-480d-82d1-6dd02fdae980)

---ผลการทดลอง `sbyte`
![Screenshot 2024-03-25 012323](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/6e207f9e-87b6-4901-9c82-a48cd3613e48)


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
![Screenshot 2024-03-25 013156](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/0775e735-e183-404d-9641-20cbb7b4132f)

## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
