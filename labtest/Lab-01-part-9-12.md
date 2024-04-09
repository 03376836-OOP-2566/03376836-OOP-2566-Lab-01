# Lab-01 การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()
### ความรู้เบื้องต้น

คำสั่งที่ใช้รับค่าตัวอักษรทางอินพุตมาตรฐานของ C# คือ Console.Read() และ Console.ReadLine() โดยทั้งสองจะมีข้อแตกต่างกันคือ Read() จะอ่านตัวอักษร ส่วน ReadLine() จะอ่านสตริงจนกว่าจะกด Enter ในการรับค่าด้วย Read() และ ReadLine() จะรับเฉพาะค่า ASCII เท่านั้น หากต้องการรับค่าตัวเลข จะต้องมีการแปลง ASCII ของตัวเลขที่พิมพ์เข้ามาให้เป็นค่าตัวเลข เช่นในการรับอักษร “22” จะไม่ได้หมายถึงค่าตัวเลข 22

## 9. การรับตัวอักษรจากคีย์บอร์ด

👉 แก้ไขโปรแกรมให้เป็นดังรูป

```csharp
char ch;
Console.Write("Press a key followed by ENTER:");
ch = (char)Console.Read();  // get a char
Console.WriteLine("Your key is: "+ch);
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/7ed6c66c-8ccd-454c-af30-5116fc59645d)


❔ ถ้าพิมพ์ตัวอักษรจำนวนหลายๆ ตัวแล้วกด Enter จะได้ผลอย่างไร ทำไมจึงเป็นเช่นนั้น
```
Console.Read(), มันจะอ่านเฉพาะตัวแรกที่พิมพ์และไม่รวม Enter (newline character) ที่ถูกส่งมาด้วย. Enter จะถูกเก็บไว้ใน buffer และถูกอ่านไปกับการเรียก Console.Read() ครั้งต่อไป
```

❔ ในบรรทัดซึ่งมีโปรแกรมเป็น ch = (char)Console.Read(); นั้น ถ้าตัด (char) ออกไป จะเกิดอะไรขึ้น ให้อธิบายประกอบ
```
ถ้าตัด (char) ออกจากบรรทัด ch = (char)Console.Read(); โปรแกรมจะยังคงทำงานได้ แต่จะเกิดปัญหาที่เกี่ยวกับประเภทข้อมูล (type) ที่ได้รับจาก Console.Read() ที่จะไม่ตรงกับตัวแปร ch ที่ถูกประกาศเป็น char
```

## 10. การรับ string จากคีย์บอร์ด

👉 แก้ไขโปรแกรมให้เป็นดังรูป

```csharp

string str;
Console.Write("Enter some characters.");
str = Console.Read();
Console.WriteLine("You entered: "+str);
```
➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/83127795-72c5-4d73-8112-761b15cdcbc6)

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

![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/981676ce-7c99-417c-92bc-97aa0f72ff93)

❔ ถ้าเราป้อนตัวอักษรลงไปแทนที่ตัวเลข จะเกิดอะไรขึ้น มีวิธีการป้องกันหรือแก้ไขอย่างไร
```
ถ้าป้อนตัวอักษรในรูปแบบที่ไม่สามารถแปลงเป็นตัวเลขได้, เช่น "abc", โปรแกรมจะ Exception ที่เกี่ยวกับการแปลงข้อมูล นอกจากนี้,ถ้าป้อนค่าที่เกินขอบเขตของข้อมูลที่สามารถแปลงได้, เช่น "12345678901234567890", จะเกิดข้อผิดพลาด (OverflowException)

เพื่อป้องกันหรือแก้ไขปัญหานี้,สามารถใช้ int.TryParse เพื่อตรวจสอบว่าป้อนเป็นตัวเลขได้หรือไม่ และป้อนได้ถูกต้องหรือไม่
ตัวอย่าง
string str;
Console.Write("Please enter value 1: ");
bool isValidInput = int.TryParse(Console.ReadLine(), out int val1);

if (isValidInput)
{
    Console.WriteLine("You entered: " + val1);
}
else
{
    Console.WriteLine("Invalid input. Please enter a valid integer.");
}
การใช้ int.TryParse จะไม่เกิดข้อผิดพลาดและค่า isValidInput จะบอกว่าการแปลงเป็นตัวเลขสำเร็จหรือไม่. ถ้าผู้ใช้ป้อนข้อมูลที่ไม่ถูกต้อง, สามารถแจ้งเตือนผู้ใช้และขอให้ป้อนใหม่.

```
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
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/b8b5e21b-17be-4c60-ba1b-f3cc105e90a6)


❔ ถ้าเราป้อนตัวอักษรลงไปแทนที่ตัวเลข จะเกิดอะไรขึ้น เหมือนหรือต่างจากโปรแกรมก่อนหน้านี้อย่างไร
```
ในโค้ดที่ให้มา, Convert.ToInt32 จะพยายามแปลงข้อมูลที่ผู้ใช้ป้อนจากคีย์บอร์ดเป็นตัวเลข (integer). ถ้าผู้ใช้ป้อนข้อมูลที่ไม่สามารถแปลงเป็นตัวเลขได้, เช่น ตัวอักษรหรือค่าที่เกินขอบเขตของ integer, จะทำให้เกิด System.FormatException ซึ่งจะถูกจับโดยบล็อก catch.
```
## 📝 แบบฝึกหัด

ให้เขียน code ในการรับค่าอินพุตต่อไปนี้และแสดงออกหน้าจอให้ถูกต้อง Name : (ป้อนชื่อของนักศึกษา)

``Lastname :`` (ป้อนนามสกุลนักศึกษา)  
``ID :`` (ป้อนรหัสนักศึกษา)  
``GPA :`` (ป้อนเกรดเฉลี่ยนักศึกษา โดยมีทศนิยมสองหลัก)  

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/b8936afc-0c65-4237-a934-7a4690a4560f)

## [การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#](./Lab-01-part-13.md)
