# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null`    | ไม่ได้ | ตั้งชื่อตัวแปรไม่ถูกต้อง  |
| `_value`  | ใช้ได้ |    ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ   |
| `First-name`| ไม่ได้ | มีตัวอักษรพิเศษที่ไม่สามารถตั้งชื่อได้ |
| `Hello!` |  ไม่ได้ | มีตัวอักษรพิเศษที่ไม่สามารถตั้งชื่อได้ |
| `w*h` |  ไม่ได้   |มีตัวอักษรพิเศษที่ไม่สามารถตั้งชื่อได้ |
| `time` |  ใช้ได้  | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ     |
| `do` |   ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ        |
| `Do` |  ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ  |
| `21November`| ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ    |
| `ladkrabang`| ใช้ได้   | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ  |
| `Student ID`| ไม่ได้   | มีช่องว่างในกฏไม่สามารถตั้งชื่อได้ |


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



![Screenshot 2024-01-27 211702](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/1b4243c8-4fe0-4f4d-aa42-ab200d81a160)



---ผลการทดลอง `byte`



![Screenshot 2024-01-27 211750](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/fc6b6aa0-6438-48ef-afa5-4ebe041eca26)



---ผลการทดลอง `short`
 


![Screenshot 2024-01-27 211826](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/0335bb72-e31d-4ade-9574-34c8c5d5eb97)




---ผลการทดลอง `ushort`

 
![Screenshot 2024-01-27 211915](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/4ab9f65c-17ba-4474-859e-2be2744faa89)






---ผลการทดลอง `uint`




![Screenshot 2024-01-27 211950](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/c37a01d1-baae-4d00-bfcd-be2d78d062cd)


 

---ผลการทดลอง `float`
 


![Screenshot 2024-01-27 212033](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/2daf6b10-b64c-46c1-be16-0eb9a9aa1015)




---ผลการทดลอง `double`




![Screenshot 2024-01-27 212119](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/9e7c8b1e-41d5-4f84-a64d-f45cb670faa2)

 
---ผลการทดลอง `decimal`


![Screenshot 2024-01-27 212202](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/7a594ba2-4381-42ab-99b8-9a975f9d2b77)



 
---ผลการทดลอง `long`


![Screenshot 2024-01-27 212236](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/5db19beb-5e41-4a6c-99c4-b42e4ca0a5a0)





---ผลการทดลอง `ulong`




![Screenshot 2024-01-27 212253](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/9f0158cf-1081-458c-a3e4-ee8fc1c1a617)



---ผลการทดลอง `bool`



![Screenshot 2024-01-27 212410](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/bcd95293-04d0-4052-9360-a22ad97ce1a5)



---ผลการทดลอง `sbyte`




![Screenshot 2024-01-27 212339](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/3a62adb1-86a9-4405-995c-cbdc511071e0)



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


![Screenshot 2024-01-27 215655](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/282acf5f-e51b-4fe3-99c5-cce0e79ffe96)



## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
