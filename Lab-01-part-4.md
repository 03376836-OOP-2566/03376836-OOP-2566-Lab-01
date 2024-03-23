# Lab-01 Part 4 จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()

โดยทั่วไป การพิมพ์ข้อความออกทาง console สามารถพิมพ์ข้อความได้ทั้งแบบตายตัวและเปลี่ยนแปลงได้โดยโปรแกรม หากเราต้องการพิมพ์แบบตายตัวก็อาจใช้คำสั่ง `Console.WriteLine` เขียนเรียงกันไปเรื่อยๆ 

👉 แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
Console.WriteLine("This is text 1.");
Console.WriteLine("This is text 2.");
Console.WriteLine("This is text 3.");
```

➢ รันโปรแกรมและบันทึกผล
<img width="861" alt="Screenshot 2024-03-23 210016" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/991b9876-c958-4750-8214-915d4040a3db">


ถ้าหากต้องการให้แก้ไขค่าตัวแปรที่จะแสดงออกทาง console เราก็อาจจะใช้ป้ายกำกับสำหรับรับค่าออกไปแสดงที่ output เรียกว่า place holder

การนับลำดับ place holder จะเริ่มจากตัวแรกที่มีค่าเป็น 0

👉 แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
Console.WriteLine(" {0} and {1}", 3, 6);
```

➢ รันโปรแกรมและบันทึกผล
<img width="859" alt="Screenshot 2024-03-23 210110" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/abbac493-396a-485d-a0ee-27df03dc235b">


❔ ถ้ามีการใช้ตัวเลขใน { } ที่กระโดด เช่น {0} {2} {3} จะใช้งานได้หรือไม่ อย่างไร จงอธิบาย
'สามารถใช้งานได้แต่ข้อมูลต้องมี4ตัวขึ้นไป'

👉แก้โปรแกรมตามรูปด้านล่างนี้

```csharp
Console.WriteLine("{1}, {0} and {1}", 3, 6);
```

➢ รันโปรแกรมและบันทึกผล
<img width="872" alt="Screenshot 2024-03-23 210137" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/954fdac5-bfa4-4433-8e2b-b3ca4dee8483">

 
## [5. การกำหนดความกว้างของอาร์กิวเมนต์](./Lab-01-part-5-7.md)
