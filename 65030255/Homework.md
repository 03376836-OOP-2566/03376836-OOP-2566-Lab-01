# 65030255 สรวิญ์ ชวนเชย
## Lab-01-part 1-15
# Part 2-3
### 2.1 การใช้เมดธอด Console.Write()
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/53f6481a-e47a-4c01-bcaa-49e3e7c4d565)

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
### -เป็นไปตามที่คิดไว้ เพราะใช้คำสั่ง Console.Write("..."); 2 รอบ แสดงผลออกมาทางคอนโทรล(ได้ข้อความติดกัน เนื่องจากไม่ได้กำหนดคำสั่งให้เว้นบรรทัด) 
### 2.2 การใช้เมดธอด Console.Write() ร่วมกับ Environment.NewLine
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/b7346add-2733-419f-9b3f-111ea038b241)

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
### -เป็นไปตามที่คิดไว้ เพราะใช้คำสั่งร่วมกับ Environment.NewLine กำหนดให้โปรแกรมขึ้นบรรทัดใหม่จึงได้ผลออกมาเป็น Hello ซึ่งอยู่คนละบรรทัดกัน
### 3. เมดธอด Console.WriteLine()
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/aa840ddb-759a-4aa2-92be-88133db62eb9)
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/19ed1967-7567-4837-b441-29e1d35cdaf1)

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
### เป็นไปตามที่คิดไว้ได้ Hello, world! ติดกัน เนื่องจากคำสั่งแรกที่ใช้คือ Console.Write ทำให้ข้อมูลที่ถูกแสดงจะต่อท้ายกับข้อมูลที่ถูกแสดงล่าสุดในบรรทัดเดียวกัน
จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
### Console.Write() ใช้เพื่อแสดงข้อมูลทางหน้าจอโดยไม่ขึ้นบรรทัดใหม่ แต่ Console.WriteLine() ใช้เพื่อแสดงข้อมูลทางหน้าจอและขึ้นบรรทัดใหม่

# Part 4
👉 แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
Console.WriteLine("This is text 1.");
Console.WriteLine("This is text 2.");
Console.WriteLine("This is text 3.");
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/5fbaebea-b2fe-4399-92cd-c822ed24a2d0)

ถ้าหากต้องการให้แก้ไขค่าตัวแปรที่จะแสดงออกทาง console เราก็อาจจะใช้ป้ายกำกับสำหรับรับค่าออกไปแสดงที่ output เรียกว่า place holder

การนับลำดับ place holder จะเริ่มจากตัวแรกที่มีค่าเป็น 0

👉 แก้โปรแกรมตามรูปด้านล่างนี้
```csharp
Console.WriteLine(" {0} and {1}", 3, 6);
```
➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/81b652a7-b619-4bd8-aca5-17782f2b334d)

❔ ถ้ามีการใช้ตัวเลขใน { } ที่กระโดด เช่น {0} {2} {3} จะใช้งานได้หรือไม่ อย่างไร จงอธิบาย
### ใช้งานได้ แต่ต้องกำหนด ข้อมูลให้เพียงพอต่อ { } สูงสุดที่เรากำหนดให้ครบด้วยเพื่อป้องกันข้อผิดพลาดและควรตรวจสอบว่า index ที่ใช้ตรงกับจำนวนข้อมูลที่เรากำหนดด้วยหรือไม่

👉แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
Console.WriteLine("{1}, {0} and {1}", 3, 6);
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/e61fec9d-dfaa-4247-ad41-d5ce15e44c00)

# Part 5-7

👉แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
Console.WriteLine("00000000011111111112");
Console.WriteLine("12345678901234567890");
Console.WriteLine("{0, 0}", 1);
Console.WriteLine("{0, 1}", 1);
Console.WriteLine("{0, 2}", 1);
Console.WriteLine("{0, 3}", 1);
Console.WriteLine("{0, 5}", 1);
Console.WriteLine("{0, 10}", 1);
Console.WriteLine("{0, 15}", 1);
Console.WriteLine("{0, 20}", 1);
```

หมายเหตุ ตัวเลขสองบรรทัดบนสุด ใช้เพื่อกำหนดตำแหน่ง column ของตัวอักษร

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/4512ec14-8100-462d-b770-f7128d2e3f75)
❔ การกำหนดความกว้างของอาร์กิวเมนต์ด้วยเครื่องหมาย { , } ในคำสั่ง ``Console.WriteLine()`` มีรูปแบบการใช้งานอย่างไร
### คือ Console.WriteLine("{index[,width]}", arg1, arg2, ...); โดย index = ตำแหน่ง index ที่จะถูกใช้แทนค่าข้อมูล width = ตำแหน่งของข้อมูลที่จะแสดงผลออกมาทางจอ

## 6. การกำหนดรูปแบบของอาร์กิวเมนต์

👉 แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
int n = 123456789;
Console.WriteLine("{0, 0:E}", n);
Console.WriteLine("{0, 0:F}", n);
Console.WriteLine("{0, 0:G}", n);
Console.WriteLine("{0, 0:N}", n);
Console.WriteLine("{0, 0:P}", n);
Console.WriteLine("{0, 0:X}", n);
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/3d467ee4-37fc-4aeb-8cc6-c4a9cde0f49d)
❔  การกำหนดตัวอักษร E, F, G, N, P, X หมายถึงให้พิมพ์ออกมาเป็นอะไร
### {0, 0:E}: แสดงเป็นตัวเลขทางวิทยาศาสตร์ (Scientific Notation)
### {0, 0:F}: แสดงเป็นทศนิยม
### {0, 0:G}: แสดงเป็นรูปแบบที่ดีที่สุดตามเงื่อนไขที่กำหนด (General Format)
### {0, 0:N}: แสดงเป็นจำนวนเต็มที่มีการคั่นหลักทุก 3 ตำแหน่ง
### {0, 0:P}: แสดงเป็นร้อยละ(%)
### {0, 0:X}: แสดงเป็นเลขฐาน 16 (Hexadecimal)
 

## 7. การกำหนดรูปแบบพร้อมความกว้างของอาร์กิวเมนต์

👉 แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
int n = 123456789;
Console.WriteLine("{0, 20:E}", 1);
Console.WriteLine("{0, 20:F}", 1);
Console.WriteLine("{0, 20:G}", 1);
Console.WriteLine("{0, 20:N}", 1);
Console.WriteLine("{0, 20:P}", 1);
Console.WriteLine("{0, 20:X}", 1);
```

➢   รันโปรแกรมและบันทึกผล
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/c2395462-27d6-4d9d-bb32-016aa7383d40)

# Part 8
👉 แก้โปรแกรมตามรูปด้านล่างนี้
```csharp
const double i = 123.456789d;
Console.WriteLine("{0:F1}", i);
Console.WriteLine("{0:F2}", i);
Console.WriteLine("{0:F3}", i);
Console.WriteLine("{0:F4}", i);
Console.WriteLine("{0:F5}", i);
```
➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/090bf55d-868c-4921-98a8-484d9b55c6cc)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/31a4012b-07ff-472a-9133-d5935d8423f4)

``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/c83c49d9-2258-41bc-a0d3-5ae6812840aa)

``` csharp
3. Console.WriteLine("Hello " + "World");
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/d5e7b7df-9e20-4396-8112-f1258b6a30e2)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/f84b354a-3276-428a-9959-859e8fe88691)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/4ab92070-a89e-4091-892b-1d5e6bc80047)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/e005d95d-e752-4c0c-a40d-9084bfa0792c)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/faf45de5-c2ad-4ba3-b83c-cb63e9525eb2)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/b813a984-1b7c-407c-a998-625dbe286b60)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/3cb6811b-e864-4f73-be96-5efbbf43e9e6)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/7cf62be0-a1b6-40d8-bef8-3a4aeb318e49)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/565c11c2-1975-4c04-9e90-20117d2ef606)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/a5834cc7-b5df-40df-8244-dfbd384b4429)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/6b804c1f-bae3-44fc-baaf-f5e19da45499)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/841cf04d-013d-4005-bbe6-f12edb65bf12)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/d7c0cd2e-8932-4af7-9301-59083a87effa)

# Part 9-12
## 9. การรับตัวอักษรจากคีย์บอร์ด

👉 แก้ไขโปรแกรมให้เป็นดังรูป

```csharp
char ch;
Console.Write("Press a key followed by ENTER:");
ch = (char)Console.Read();  // get a char
Console.WriteLine("Your key is: "+ch);
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/55fe7adb-96ae-4afc-87d9-ca04f51ff4c0)


❔ ถ้าพิมพ์ตัวอักษรจำนวนหลายๆ ตัวแล้วกด Enter จะได้ผลอย่างไร ทำไมจึงเป็นเช่นนั้น
### ถ้ากดตัวอักษรหลายตัวจะแสดง ตัวอักษรตัวเดียว คือ ตัวแรก
❔ ในบรรทัดซึ่งมีโปรแกรมเป็น ch = (char)Console.Read(); นั้น ถ้าตัด (char) ออกไป จะเกิดอะไรขึ้น ให้อธิบายประกอบ
### ถ้าตัด char ออก Input ที่ผู้ใช้งานป้อนเข้ามาจะมีปัญหาเนื่องจากไม่รู้ ชนิดข้อมูลที่ถูกป้อนเข้ามา

## 10. การรับ string จากคีย์บอร์ด

👉 แก้ไขโปรแกรมให้เป็นดังรูป

```csharp
string str;
Console.Write("Enter some characters.");
str = Console.Read();
Console.WriteLine("You entered: "+str);
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/40d3ffa8-0da1-4f28-a0ef-80554470637c)

## 11. การรับค่าตัวเลขจากคีย์บอร์ด

เนื่องจากคำสั่ง Read() และ ReadLine() จะรับเฉพาะตัวอักษร การรับตัวเลข เราต้องใช้เมธอด TryParse() มาช่วยแปลงค่า

👉 แก้ไขโปรแกรมให้เป็นดังรูป

```csharp
string str;
Console.Write("Please enter value 1 : ");
int val1 = Convert.ToInt32(Console.ReadLine());
Console.WriteLine(val1);
```

➢ รันโปรแกรม โดยป้อนตัวเลขใดๆ และบันทึกผลที่ได้
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/4479fc39-ac96-4f4e-8e4a-ab9f54e98f4f)


❔ ถ้าเราป้อนตัวอักษรลงไปแทนที่ตัวเลข จะเกิดอะไรขึ้น มีวิธีการป้องกันหรือแก้ไขอย่างไร
### เกิด Error อาจใช้คำสั่งแปลงชนิดข้อมูลอย่าง try/tryParse และอื่นๆเข้ามาช่วย

## 12. การรับค่าตัวเลขจากคีย์บอร์ด (ป้องกันโดยใช้ประโยค try{…} catch{…})

ในบางกรณีที่ผู้ใช้ป้อนตัวอักษร จะทำให้เกิด error และทำให้โปรแกรม hang ได้ จึงต้องมีการป้องกันโดยใช้ประโยค `try{…}` `catch{…}` (ประโยค `try{…}` `catch{…}`   นี้จะศึกษารายละเอียดภายหลัง)

👉 แก้ไขโปรแกรมให้เป็นดังรูป

```csharp
try
{
    Console.Write("Please enter value 1 :");
    int val1 = Convert.ToInt32(Console.ReadLine());
    Console.Write("Please enter value 2 :");
    int val2 = Convert.ToInt32(Console.ReadLine());
    Console.WriteLine("Answer = " + (val1 + val2));
}
catch (Exception e)
{
    Console.WriteLine("Error : " + e.ToString());
}
```

➢ รันโปรแกรม โดยป้อนตัวเลขใดๆ และบันทึกผล
![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/f18c1c14-5838-453d-9fad-d3acb521b55b)


❔ ถ้าเราป้อนตัวอักษรลงไปแทนที่ตัวเลข จะเกิดอะไรขึ้น เหมือนหรือต่างจากโปรแกรมก่อนหน้านี้อย่างไร
### Error เหมือนกันต่างกันตรงที่โปแรกรมนี้เราได้เขียนป้องกันเผื่อข้อมูลที่รับมาเป็นstr จะขึ้นแจ้งเตือนไป ไม่เด้งหลุดโปรแกรมเหมือนก่อนหน้า

## 📝 แบบฝึกหัด

ให้เขียน code ในการรับค่าอินพุตต่อไปนี้และแสดงออกหน้าจอให้ถูกต้อง Name : (ป้อนชื่อของนักศึกษา)

``Lastname :`` (ป้อนนามสกุลนักศึกษา)  
``ID :`` (ป้อนรหัสนักศึกษา)  
``GPA :`` (ป้อนเกรดเฉลี่ยนักศึกษา โดยมีทศนิยมสองหลัก)  

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/01aa4970-1c1b-4124-9d82-1a3a3026ba46)




