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

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/cc033d2a-371e-4158-acea-421d7632beb6)

❔ ถ้าพิมพ์ตัวอักษรจำนวนหลายๆ ตัวแล้วกด Enter จะได้ผลอย่างไร ทำไมจึงเป็นเช่นนั้น

Console.Read() จะอ่านตัวอักษรตัวแรกที่ป้อนและปล่อยตัวอักษรที่เหลือในบัฟเฟอร์ เพราะ enter นับว่าเป็นตัวอักษรแบบพิเศษ

❔ ในบรรทัดซึ่งมีโปรแกรมเป็น ch = (char)Console.Read(); นั้น ถ้าตัด (char) ออกไป จะเกิดอะไรขึ้น ให้อธิบายประกอบ
ยังทำงานได้เหมือนเดิมแต่ตัวแปลจะรับค่า int แทน char เพราะไม่ถูกแปลงค่า

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/1fe7a11d-4931-4bc6-b2a0-c17854cafce3)

## 10. การรับ string จากคีย์บอร์ด

👉 แก้ไขโปรแกรมให้เป็นดังรูป

```csharp
string str;
Console.Write("Enter some characters.");
str = Console.Read();
Console.WriteLine("You entered: "+str);
```

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/15c6f3ea-a742-4775-9bc7-134fffde01aa)

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

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/bf1df17f-a04e-4d20-b0ca-1c2026892961)

❔ ถ้าเราป้อนตัวอักษรลงไปแทนที่ตัวเลข จะเกิดอะไรขึ้น มีวิธีการป้องกันหรือแก้ไขอย่างไร

code error วิธีป้องกันคือใช้ char แทน int
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

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/b01adab6-337e-45c2-acfc-448f9bc6abf3)

❔ ถ้าเราป้อนตัวอักษรลงไปแทนที่ตัวเลข จะเกิดอะไรขึ้น เหมือนหรือต่างจากโปรแกรมก่อนหน้านี้อย่างไร

code error แตกต่างเพราะโปรแกรมนี้มีการรับค่า 2 ค่า แล้วนนำมาแสดงผล
## 📝 แบบฝึกหัด

ให้เขียน code ในการรับค่าอินพุตต่อไปนี้และแสดงออกหน้าจอให้ถูกต้อง Name : (ป้อนชื่อของนักศึกษา)

``Lastname :`` (ป้อนนามสกุลนักศึกษา)  
``ID :`` (ป้อนรหัสนักศึกษา)  
``GPA :`` (ป้อนเกรดเฉลี่ยนักศึกษา โดยมีทศนิยมสองหลัก)  

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/aa7b5d33-853d-43e7-8dc5-830dc1a40fd3)

## [การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#](./Lab-01-part-13.md)
