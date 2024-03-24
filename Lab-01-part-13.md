# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null` |ใช้ไม่ได้ |เป็นคำสงวน |
| `_value` |ใช้ได้ |ถูกตามหลัก |
| `First-name`|ใช้ไม่ได้ |มีอักขระพิเศษ |
| `Hello!` |ใช้ไม่ได้ |มีอักขระพิเศษ |
| `w*h` |ใช้ไม่ได้ |มีอักขระพิเศษ |
| `time` |ใช้ได้ |ถูกตามหลัก |
| `do` |ใช้ไม่ได้ |เป็นคำสงวน |
| `Do` |ใช้ได้ |ถูกตามหลัก |
| `21November`|ใช้ไม่ได้ |ตัวเลขนำหน้าไม่ได้ |
| `ladkrabang`|ใช้ได้ |ถูกตามหลัก |
| `Student ID`|ใช้ไม่ได้ |มีการเว้นว่าง  |



---ผลการทดลอง
## ![Screenshot 2024-03-23 222157](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/480d6207-30a0-4753-abe6-2a3167c0dffc)

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
<img width="859" alt="Screenshot 2024-03-23 230447" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/c128a894-dcef-4998-828b-e00ad4b901f6">
---ผลการทดลอง `byte`
<img width="859" alt="Screenshot 2024-03-23 230447" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/c128a894-dcef-4998-828b-e00ad4b901f6">
---ผลการทดลอง `short`
 <img width="859" alt="Screenshot 2024-03-23 230748" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/2c1446f4-bb66-4576-894e-dab3c5712b2e">

---ผลการทดลอง `ushort`
<img width="859" alt="Screenshot 2024-03-23 230748" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/2c1446f4-bb66-4576-894e-dab3c5712b2e">
 

---ผลการทดลอง `uint`
<img width="852" alt="Screenshot 2024-03-23 230921" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/cb768980-2fb4-4dc8-adb4-a5301a22c875">

 

---ผลการทดลอง `float`
 <img width="863" alt="Screenshot 2024-03-23 231007" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/679a1195-13ee-498b-accc-11d5a28dbf2f">


---ผลการทดลอง `double`
 <img width="854" alt="Screenshot 2024-03-23 231106" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/c4d23275-22c2-4bae-b976-90e8acd13a63">

---ผลการทดลอง `decimal`
 <img width="857" alt="Screenshot 2024-03-23 231213" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/2828c8c1-eeb1-4e45-aafe-29e43ac99d9c">

---ผลการทดลอง `long`
<img width="857" alt="Screenshot 2024-03-23 231248" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/936dd367-97ff-46d9-8d5a-847871347822">


---ผลการทดลอง `ulong`
<img width="851" alt="Screenshot 2024-03-23 231306" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/b6c570ee-fb42-4ab1-9f97-89910e66411b">


---ผลการทดลอง `bool`

---ผลการทดลอง `sbyte`
<img width="860" alt="Screenshot 2024-03-23 231554" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/882cab61-2692-483a-b8f5-6ff15e7420e5">


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
<img width="854" alt="Screenshot 2024-03-23 231739" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/9cb3b0c2-9aef-413d-b362-326aebcaaf21">
<img width="856" alt="Screenshot 2024-03-23 231750" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/f6214a68-452a-42da-83b7-d452444b28d6">
<img width="860" alt="Screenshot 2024-03-23 231758" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/0bd1650b-33ab-4726-9344-e644093faa42">
<img width="855" alt="Screenshot 2024-03-23 231807" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/35692a5c-60dc-4aa2-befc-c4d7bb17d0ad">
<img width="848" alt="Screenshot 2024-03-23 231817" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/0c44611c-c285-43b2-810b-4e31cde8fb7f">
<img width="851" alt="Screenshot 2024-03-23 231827" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/8aa02446-6815-42bb-b48e-71d40e75f4d2">
<img width="851" alt="Screenshot 2024-03-23 231837" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/77aea34e-fb28-432d-884a-39955d95359f">
<img width="848" alt="Screenshot 2024-03-23 231851" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/aa778b4e-b70e-4856-9293-b80d182277a2">
<img width="851" alt="Screenshot 2024-03-23 231900" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/7142361c-6e5b-44dc-80b7-cd0e41c991b5">
<img width="853" alt="Screenshot 2024-03-23 231911" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/5eababbc-8050-413e-ac95-932ec57e19d7">

## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
