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
## ![Screenshot 2024-03-23 224241](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/50474949-9983-41bb-9884-edfb7869fcd1)

---ผลการทดลอง `byte`
## ![Screenshot 2024-03-23 224302](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/42f1c541-68e8-444a-910b-cf2650cdf88b)

---ผลการทดลอง `short`
## ![Screenshot 2024-03-23 224331](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/823cd506-86d9-4407-90ad-7bd175df0d9f)


---ผลการทดลอง `ushort`
## ![Screenshot 2024-03-23 224349](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/ec40188f-8fbd-4413-b176-565935069b54)

 

---ผลการทดลอง `uint`
## ![Screenshot 2024-03-23 224407](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/4d72721d-1de6-42c0-ac33-84a57dac307b)

 

---ผลการทดลอง `float`
## ![Screenshot 2024-03-23 224427](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/0fdba1bd-6c6e-449d-9b73-beab49b4092e)


---ผลการทดลอง `double`
## ![Screenshot 2024-03-23 224629](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/8a92f05b-66f4-412c-9b41-c6c7cc7e3910)

---ผลการทดลอง `decimal`
## ![Screenshot 2024-03-23 224647](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/f6873462-6cc9-4ece-be37-1ae4dfe29ff9)

---ผลการทดลอง `long`
## ![Screenshot 2024-03-23 224739](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/0e2ea829-befa-4f6d-81be-1573e1b42a6d)


---ผลการทดลอง `ulong`
## ![Screenshot 2024-03-23 224754](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/42c47165-9e2e-4d14-9d88-8c82862d860d)


---ผลการทดลอง `bool`

---ผลการทดลอง `sbyte`
## ![Screenshot 2024-03-23 224858](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/32468406-7916-4465-b5ae-a26ea067f5e7)


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
## ![Screenshot 2024-03-23 225639](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/f8b70cec-6460-4ca5-92e1-1574131677ac)

## ![Screenshot 2024-03-23 225652](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/74c907f0-2ecf-40ab-a86d-0828ed6cd0a9)

## ![Screenshot 2024-03-23 225704](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/6f2bb80c-0817-45f8-90fd-fb666406877b)

## ![Screenshot 2024-03-23 225713](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/c748a9db-0fdb-4bda-84ae-f800d50d6084)

## ![Screenshot 2024-03-23 225721](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/c2222000-4983-497c-a4cd-c5960fd95e97)

## ![Screenshot 2024-03-23 225730](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/f91d33c9-2178-4166-b7b1-8e29d4cb5755)

## ![Screenshot 2024-03-23 225740](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/c7efbee0-342b-47cf-bd8e-92b4b08588c3)

## ![Screenshot 2024-03-23 225748](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/b9ab720f-7acf-44b9-88f7-09577411a505)

## ![Screenshot 2024-03-23 225757](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/76fdf996-c10b-48ac-9c22-af19c41079a0)

## ![Screenshot 2024-03-23 225813](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/f5a5cd23-6af4-4e07-b29e-12dd948fc897)


## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
