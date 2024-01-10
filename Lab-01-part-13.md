# Lab-01 การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#


 ให้นักศึกษาพิจารณาชื่อตัวแปรตามตารางต่อไปนี้ ว่าสามารถใช้ได้หรือไม่ พร้อมบอกเหตุผล

| ชื่อตัวแปร | ใช้ได้/ไม่ได้ | เหตุผล|
|--|--|--|
| `xxx`     | ใช้ได้ | ไม่มีตัวอักษรที่ละเมิดกฎการตั้งชื่อ |
| `null` | ไม่ได้  | นื่องจากชื่อตัวแปร null ละเมิดกฎการตั้งชื่อ|
| `_value` | ใช้ได้| เนื่องจากชื่อตัวแปร value เป็นไปตามกฎการตั้งชื่อ |
| `First-name`|ใช้ได้  |เนื่องจากชื่อตัวแปร First-name เป็นไปตามกฎการตั้งชื่อของ |
| `Hello!` |ไม่ได้ |เนื่องจากชื่อตัวแปร Hello! ละเมิดกฎการตั้งชื่อของ |
| `w*h` |ไม่ได้  |เนื่องจากชื่อตัวแปร wh ละเมิดกฎการตั้งชื่อ |
| `time` |ใช้ได้ |เนื่องจากชื่อตัวแปร time เป็นไปตามกฎการตั้งชื่อ |
| `do` |ใช้ได้ |เนื่องจากชื่อตัวแปร do เป็นไปตามกฎการตั้งชื่อ |
| `Do` |ใช้ได้ |เนื่องจากชื่อตัวแปร Do เป็นไปตามกฎการตั้งชื่อ |
| `21November`|ไม่ได้ |เนื่องจากชื่อตัวแปร 21 November ละเมิดกฎการตั้งชื่อของภาษ |
| `ladkrabang`|ใช้ได้ |เนื่องจากชื่อตัวแปร ladkrang เป็นไปตามกฎการตั้งชื่อ |
| `Student ID`|ใช้ได้  |เนื่องจากชื่อตัวแปร Student ID เป็นไปตามกฎการตั้งชื่อ |


---ผลการทดลอง
โดยสรุปแล้ว เฉพาะชื่อตัวแปร XXX, value, time, ladkrang และ Student ID เท่านั้นที่สามารถใช้ได้

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
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/27e27880-e250-4b1f-8efd-6ad37c49cb44)

---ผลการทดลอง `byte`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/76187729-814e-4ae8-85fd-86c0ccc06cfd)

---ผลการทดลอง `short`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/bb17128c-d73e-40a6-bab6-2dce43b4436e)



---ผลการทดลอง `ushort`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/d48ea9e5-279b-468c-a441-857dc6e621a3)

 

---ผลการทดลอง `uint`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/40097c6f-e636-4e7f-bbca-858df4fb87ea)

 

---ผลการทดลอง `float`
 ![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/5a58c0d0-98e5-473b-ba0a-b1fde8cea5db)


---ผลการทดลอง `double`
 ![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/d11e6408-fb90-4979-979f-c3abd078e780)

---ผลการทดลอง `decimal`
 ![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/e081743f-abb5-4f0d-ace4-a3341ebc0e2e)

---ผลการทดลอง `long`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/94a11e7c-af40-4315-bfcf-6af7d8e1c4d7)


---ผลการทดลอง `ulong`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/98bbbe24-964e-4de2-a963-4404267ec5dd)


---ผลการทดลอง `bool`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/c95554b6-d0c8-47a8-80aa-542af2b6c77a)

---ผลการทดลอง `sbyte`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/a5b61ac4-8102-46fa-b085-d8b1b29db02f)


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
1![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/3660b194-8cb6-444e-bd2c-2b1584265889)
2![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/1dc0e8c2-9530-4069-a7f2-83de567152be)
3![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/7a2da5d6-bbed-4953-9420-e926170f4bf3)
4![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/2b8caf0f-7da4-4227-b6b5-de6232f3a949)
5![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/ef888c1f-27cc-4d7d-ae24-303472c2fe5b)
6![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/9a7ccdbf-f115-42f9-98aa-d8c719522028)
7![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/42fd48e4-c361-494a-81a7-5f01a2ddb15a)
8![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/d27e6e97-ae2f-454c-b141-6d5a7d076ccd)
9![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/e76ecb53-4b1b-47a1-84fa-b4684208abd2)
10![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/795e4ba7-8664-4161-979f-5163d38b8f3f)


## [การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ](./Lab-01-part-14.md)
