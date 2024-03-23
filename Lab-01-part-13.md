# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null` | ใช้ไม่ได้ | มีคำที่ซ้อนกับnull |
| `_value` | ใช้ได้ | ถูกตามหลักสร้างตัวแปร |
| `First-name`| ใช้ไม่ได้ | มีเครื่องหมายทางคณิตศาสตร์ |
| `Hello!` | ใช้ไม่ได้ | มีเครืื่องหมายพิเศษ |
| `w*h` | ใช้ไม่ได้ | มีเครื่องหมายทางคณิตศาสตร์ |
| `time` | ใช้ได้ | ถูกตามหลักการสร้างตัวแปร |
| `do` | ใช้ไม่ได้ | เป็นคำสงวน |
| `Do` | ใช้ได้ | ถูกตามหลักการสร้างตัวแปร |
| `21November`| ใช้ไม่ได้ | มีตัวเลขนำหน้า |
| `ladkrabang`| ใช้ได้ | ถูกตามหลักการสร้างตัวแปร |
| `Student ID`| ใช้ไม่ได้ | มีการเว้นช่องว่าง |


---ผลการทดลอง

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/a9fcc7c0-9f0a-4f4a-a582-6add35bcd078)

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

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/8131aa2e-27a7-4deb-ae04-455f75ba4627)

---ผลการทดลอง `byte`

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/c03aec7b-3170-4748-ac54-b9e9bddd74c5)

---ผลการทดลอง `short`
 
![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/626475b8-a8d4-44a2-91d8-c47a8242c5fc)

---ผลการทดลอง `ushort`

 ![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/59ab4114-7dec-4945-ab27-80fca1fe0912)


---ผลการทดลอง `uint`

 ![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/4fec6b45-6538-4cb0-bac8-cc21c8e278a6)


---ผลการทดลอง `float`
 
![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/1511f549-2c4d-464d-a4ec-4ccb4b45417d)

---ผลการทดลอง `double`

 ![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/035b538a-9382-4749-bdae-5a987b6bc4f4)

---ผลการทดลอง `decimal`

 ![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/0c46e5b0-1392-41da-b0ff-945ce46bafdc)

---ผลการทดลอง `long`

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/0c638c81-46fd-4807-ba19-868c8eb97b3c)

---ผลการทดลอง `ulong`

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/169ea0c3-8ab3-428a-ae64-ad2bcb992606)

---ผลการทดลอง `bool`


---ผลการทดลอง `sbyte`

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/f452277f-5630-4595-9717-ba3b46723fa0)

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
![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/5fb125c8-1425-4da8-ac31-6c9d6a934ac9)

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/37a5f4a9-ecb5-4c87-993b-98e20a6298da)

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/5c4e3a70-a090-4d4e-b96c-78c5c552cd18)

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/6468d21d-421e-42c1-afab-30af81532794)

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/e47f539e-1ce8-43d9-971c-5721e79f9668)

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/c8643443-40ab-40ba-b402-981aa3dd3d21)

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/6e499b4a-216e-4188-b405-a7af965a1a85)

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/5b4c4e39-6ad5-406a-9e64-2b15821fca23)

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/7905b9e0-dd12-4659-a974-553b56c5f84c)

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/b9a54356-460d-40b1-986e-4cc17a96f3c0)





















## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
