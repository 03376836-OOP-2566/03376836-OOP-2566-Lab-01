# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null` | ใช้ไม่ได้| มีคำสั่งที่ซ้อนกับnull|
| `_value` | ใช้ได้ | ถูกตามหลักสร้างตัวแปร|
| `First-name`|ใช้ไม่ได้ |มีเครื่องหมายทางคณิตศาสตร์ |
| `Hello!` | ใช้ไม่ได้ |มีเครื่องหมายอัศเจรีย์ |
| `w*h` | ใช้ไม่ได้ |มีเครื่องหมายทางคณิตศาสตร์ |
| `time` | ใช้ได้ |ถูกตามหลักสร้างตัวแปร |
| `do` | ใช้ไม่ได้ | มีคำสั่งที่ซ้อนกับdo|
| `Do` | ใช้ได้ |ถูกตามหลักสร้างตัวแปร |
| `21November`| ใช้ไม่ได้ | ตัวเลขนำหน้าไม่ได้|
| `ladkrabang`| ใช้ได้ | ถูกตามหลักสร้างตัวแปร|
| `Student ID`| ใช้ไม่ได้ | มีการเว้นว่าง |


---ผลการทดลอง
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/32bee9fa-5c45-4272-8b87-024a6a3eaec8)


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
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/7d1da8e8-8a42-4253-80c5-c13180929763)

---ผลการทดลอง `byte`
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/e732b6a4-d822-4d28-9bc6-48ec8844f4cd)

---ผลการทดลอง `short`
 ![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/a67cf7d2-c538-4896-9344-bb4c985f3230)


---ผลการทดลอง `ushort`
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/441e7d31-7de2-4bd7-88b9-e9ee28708dcc)

 

---ผลการทดลอง `uint`
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/98b273cc-9079-46e6-83ba-94bcf31a4247)

 

---ผลการทดลอง `float`
 ![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/58cd9bed-2828-4098-af5a-0dd1edabb8ef)


---ผลการทดลอง `double`
 ![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/36c3a2b0-1982-4a3f-8121-721f1a2dc92a)

---ผลการทดลอง `decimal`
 ![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/34b1f633-23e2-4f1f-9da0-37ee5042496c)

---ผลการทดลอง `long`
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/368486b9-d1b6-42ce-8f09-6da382084c5a)


---ผลการทดลอง `ulong`
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/74515a0e-5846-4b30-9caf-4b1c4bddf99f)


---ผลการทดลอง `bool`
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/6ab16904-7e6c-4c5d-8336-2184b0344126)

---ผลการทดลอง `sbyte`
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/fd55a3e4-e5ea-4a5f-94df-7287670900ae)


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
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/685087d5-48b5-40d9-a36b-3312d76cc1f7)

## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
