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
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/e2ea1155-7a5b-46d5-bc07-195900028e2c)

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
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/c2c29cdf-cf8c-4b13-b6fa-35c3ccfb0b10)

---ผลการทดลอง `byte`
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/d8b209a1-1a20-4967-93a0-d5d65b7109e8)

---ผลการทดลอง `short`
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/f36bb604-9c63-419e-a6ec-98df47ad0399)
 
---ผลการทดลอง `ushort`
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/ba87f46d-8454-4466-a78b-0db95e1af5ad)

---ผลการทดลอง `uint`
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/59ae3da3-da86-4b5f-a8a1-f9c356b56cb9)

---ผลการทดลอง `float`
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/81d15b4d-0684-43b0-ae3c-ba33e9b7302d)
 
---ผลการทดลอง `double`
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/bb2792d0-9fa6-4fd6-add3-4866125fbce7)
 
---ผลการทดลอง `decimal`
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/8b1f27b4-9852-4a84-8ba6-c382756e663b)
 
---ผลการทดลอง `long`
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/76db6e0f-da61-4c00-b46e-7cd2d96a9549)

---ผลการทดลอง `ulong`
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/edc783c2-9940-4393-a7d2-226c3666fb66)

---ผลการทดลอง `bool`

---ผลการทดลอง `sbyte`
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/16e3ba85-e165-4ce7-87a8-8c71fd1be910)


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
![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/4c26afdc-f410-468a-a209-86f6135ac7de)

![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/fdd70943-a075-4e60-a29b-fbbbabf08d76)

![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/bebd5427-f58e-4ef4-99ca-f2e2ab086655)

![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/7d43f31b-0c16-403d-82c6-b2df89145ddb)

![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/7be25402-63ec-4337-8083-7547403c2de1)

![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/8c1b4d3b-34d2-4ad7-9d91-b039cb506df9)

![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/d3b0bce7-58c9-4346-8691-c72e1b8ef94a)

![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/f895d011-d8fe-4daf-8c3e-6cf527e65f97)

![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/b307f37c-1aee-4f7b-8fed-be41dff41966)

![image](https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/9d5cb4cf-d5bd-4f29-8a2b-d552f4fb9cab)

## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
