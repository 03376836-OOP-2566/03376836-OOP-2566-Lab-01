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
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/f91e496c-c256-4407-85b5-e721243806b8)


❔ ถ้าพิมพ์ตัวอักษรจำนวนหลายๆ ตัวแล้วกด Enter จะได้ผลอย่างไร ทำไมจึงเป็นเช่นนั้น
ตอบ เเสดงผลตัวอักษรตัวเเรก
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/fbfc21f5-3744-485e-b1c4-66949bd81d4b)



❔ ในบรรทัดซึ่งมีโปรแกรมเป็น ch = (char)Console.Read(); นั้น ถ้าตัด (char) ออกไป จะเกิดอะไรขึ้น ให้อธิบายประกอบ
ตอบ
อธิบาย:
'int': เป็นชนิดข้อมูล (data type) ที่ใช้เก็บตัวเลขเต็ม (ทั้งบวก ลบ และ 0)
'char': เป็นชนิดข้อมูลที่ใช้เก็บอักขระเดี่ยว ๆ (เช่น ตัวอักษร ตัวเลข สัญลักษณ์)
ข้อผิดพลาดนี้เกิดขึ้นเมื่อคุณพยายามกำหนดค่าตัวเลขเต็ม (int) ให้กับตัวแปรที่ประกาศเป็นประเภท 'char' โดยตรง ในภาษา C#, การกำหนดค่าโดยตรงระหว่างชนิดข้อมูลที่ต่างกันนั้นมักจะไม่สามารถทำได้โดยอัตโนมัติ (implicitly) เพราะอาจส่งผลต่อข้อมูลหรือทำให้โปรแกรมทำงานผิดพลาด เเสดงผลดังรูป
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/62ab1e95-bf86-46b3-ad63-f3dba2d7d278)


## 10. การรับ string จากคีย์บอร์ด

👉 แก้ไขโปรแกรมให้เป็นดังรูป

```csharp
string str;
Console.Write("Enter some characters.");
str = Console.Read();
Console.WriteLine("You entered: "+str);
```

➢ รันโปรแกรมและบันทึกผล
ไม่สามารถรันโปรเเกรมได้
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/4eb3ceaf-6d8b-4ecc-aabd-65fb680fadd6)


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
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/bea96e94-882a-4629-a3c3-e191420575e2)


❔ ถ้าเราป้อนตัวอักษรลงไปแทนที่ตัวเลข จะเกิดอะไรขึ้น มีวิธีการป้องกันหรือแก้ไขอย่างไร
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/1a263e66-a722-4ae3-b9ca-61335f1d2bbf)


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
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/438921d7-f02c-4a16-a270-57a642b7fa59)


❔ ถ้าเราป้อนตัวอักษรลงไปแทนที่ตัวเลข จะเกิดอะไรขึ้น เหมือนหรือต่างจากโปรแกรมก่อนหน้านี้อย่างไร
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/f71fd488-2669-4f12-ae31-0b0fdc3ef630)


## 📝 แบบฝึกหัด

ให้เขียน code ในการรับค่าอินพุตต่อไปนี้และแสดงออกหน้าจอให้ถูกต้อง Name : (ป้อนชื่อของนักศึกษา)

``Lastname :`` (ป้อนนามสกุลนักศึกษา)  
``ID :`` (ป้อนรหัสนักศึกษา)  
``GPA :`` (ป้อนเกรดเฉลี่ยนักศึกษา โดยมีทศนิยมสองหลัก)  

➢ รันโปรแกรมและบันทึกผล

## [การตั้งชื่อตัวแปรและชนิดข้อมูลในภาษา C\#](./Lab-01-part-13.md)
