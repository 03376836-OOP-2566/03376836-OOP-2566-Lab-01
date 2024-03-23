# Lab-01 Part 2~3 คำสั่ง Console.Write() และ Console.WriteLine()

## 2. การใช้เมดธอด Console.Write()

### 2.1 การใช้เมดธอด Console.Write()
👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello");
Console.Write("Hello");
```

➢ รันโปรแกรมและบันทึกผล

![Screenshot 2024-01-18 135328](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/50a66055-5087-4639-85da-49f965916739)

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย

👉👉ตามที่คิดไว้เพราะสั่งไป 2 ครั้งโดยเป็นการสั่งต่อกัน จึงได้แสดงคำว่า HelloHello ต่อกัน
### 2.2 การใช้เมดธอด Console.Write() ร่วมกับ  `Environment.NewLine`

`Environment.NewLine` เป็นค่าคงที่ที่ถูกนิยามในภาษา C# เพื่อใช้สำหรับการส่งอักขระขึ้นบรรทัดใหม่ไปยัง console

👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello" + Environment.NewLine);
Console.Write("Hello" + Environment.NewLine);
```

➢ รันโปรแกรมและบันทึกผล
![Screenshot 2024-01-18 135438](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/9ce26e29-3034-4345-860d-3a306028eda8)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย

👉👉ขึ้นบรรทัดใหม่คำว่า Hello ตามที่กำหนดด้วย Environment.NewLine ทำให้เกิดการขึ้นบรรทัดใหม่
## 3. เมดธอด Console.WriteLine()

`Console.WriteLine()` เป็นคำสั่งที่เทียบเท่ากับการใช้  `Console.Write` ร่วมกับ  `Environment.NewLine` ทำให้ประหยัดเวลาในการเขียนโปรแกรม
👉 แก้โปรแกรมในเมดธอด Main() ให้เป็นดังต่อไปนี้

```csharp
Console.WriteLine("Hello");
```

➢ รันโปรแกรมและบันทึกผล
![Screenshot 2024-01-18 135912](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/b32fcfbe-749d-45ca-9c76-87abdaf237b7)


👉 แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

```csharp
Console.Write("Hello, ");
Console.WriteLine("World!");
```

➢ รันโปรแกรมและบันทึกผล
![Screenshot 2024-01-18 135942](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/1ec17e3a-cbc3-42ce-ae24-3fabb617b081)

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
👉👉จะแสดงผลลัพธ์ "Hello, " บน console โดยไม่ขึ้นบรรทัดใหม่ และตามด้วย "World!" บนบรรทัดใหม่ โดยใช้ Console.Write เพื่อพิมพ์ "Hello, " โดยไม่ขึ้นบรรทัดใหม่ และ Console.WriteLine เพื่อพิมพ์ "World!" 

❔ จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
👉👉ความแตกต่างสำคัญระหว่าง Console.Write() และ Console.WriteLine() คือ Console.Write() จะไม่ขึ้นบรรทัดใหม่หลังจากการแสดงข้อความเสร็จสิ้น ในขณะที่ Console.WriteLine() จะขึ้นบรรทัดใหม่หลังจากการแสดงข้อความเสร็จสิ้นในแต่ละครั้งที่เรียกใช้งาน ทำให้ข้อความถัดไปที่ถูกแสดงจะอยู่บนบรรทัดใหม่ในกรณีของ Console.WriteLine() ลงไปที่ถัดไปในคำสั่ง ในขณะที่ในกรณีของ Console.Write() ข้อความถัดไปจะถูกแสดงบนบรรทัดเดียวกันกับข้อความก่อนหน้านี้โดยไม่มีการขึ้นบรรทัดใหม่ทันทีหลังจากการแสดงผลลัพธ์

## [4. จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()](./Lab-01-part-4.md)
