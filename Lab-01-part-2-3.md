# Lab-01 Part 2~3 คำสั่ง Console.Write() และ Console.WriteLine()

## 2. การใช้เมดธอด Console.Write()

### 2.1 การใช้เมดธอด Console.Write()
👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello");
Console.Write("Hello");
```

➢ รันโปรแกรมและบันทึกผล

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
<img width="723" alt="Screenshot 2024-03-23 193659" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/5d7e7c58-5da3-4d14-89a7-42a5b1a25da2">

แสดง Hello ในบรรทัดเดียวกัน

### 2.2 การใช้เมดธอด Console.Write() ร่วมกับ  `Environment.NewLine`

`Environment.NewLine` เป็นค่าคงที่ที่ถูกนิยามในภาษา C# เพื่อใช้สำหรับการส่งอักขระขึ้นบรรทัดใหม่ไปยัง console

👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello" + Environment.NewLine);
Console.Write("Hello" + Environment.NewLine);
```

➢ รันโปรแกรมและบันทึกผล

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
<img width="718" alt="Screenshot 2024-03-23 193723" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/5f07c768-98d1-4b19-aa71-07a6e4a1591a">

แสดง Hello โดยการขึ้นบรรทัดใหม่

## 3. เมดธอด Console.WriteLine()

`Console.WriteLine()` เป็นคำสั่งที่เทียบเท่ากับการใช้  `Console.Write` ร่วมกับ  `Environment.NewLine` ทำให้ประหยัดเวลาในการเขียนโปรแกรม
👉 แก้โปรแกรมในเมดธอด Main() ให้เป็นดังต่อไปนี้

```csharp
Console.WriteLine("Hello");
```

➢ รันโปรแกรมและบันทึกผล
<img width="719" alt="Screenshot 2024-03-23 193738" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/109d0331-d43c-434f-a9ed-8d462e2eaa19">

👉 แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

```csharp
Console.Write("Hello, ");
Console.WriteLine("World!");
```

➢ รันโปรแกรมและบันทึกผล
<img width="713" alt="Screenshot 2024-03-23 193752" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/2adfa7d0-ccfc-4d73-80be-7c1ed8af7d05">

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
Hello, และ World! จะแสดงผลในบรรทัดเดียววัน

❔ จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
'Console.Write() จะแสดงคำให้อยู่ในบรรทัดเดียวกัน แต่ Console.WriteLine() จะเป็นการขึ้นบรรทัดใหม่'

## [4. จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()](./Lab-01-part-4.md)
