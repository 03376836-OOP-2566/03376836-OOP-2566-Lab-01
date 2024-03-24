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
<img width="857" alt="Screenshot 2024-03-23 205704" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/704aefa1-db77-4e7a-9bdf-832c6cf48daa">

### 2.2 การใช้เมดธอด Console.Write() ร่วมกับ  `Environment.NewLine`

`Environment.NewLine` เป็นค่าคงที่ที่ถูกนิยามในภาษา C# เพื่อใช้สำหรับการส่งอักขระขึ้นบรรทัดใหม่ไปยัง console

👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello" + Environment.NewLine);
Console.Write("Hello" + Environment.NewLine);
```

➢ รันโปรแกรมและบันทึกผล


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
<img width="850" alt="Screenshot 2024-03-23 205722" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/ae2381d7-c679-4465-8d5b-0c73f9aa5162">


## 3. เมดธอด Console.WriteLine()

`Console.WriteLine()` เป็นคำสั่งที่เทียบเท่ากับการใช้  `Console.Write` ร่วมกับ  `Environment.NewLine` ทำให้ประหยัดเวลาในการเขียนโปรแกรม
👉 แก้โปรแกรมในเมดธอด Main() ให้เป็นดังต่อไปนี้

```csharp
Console.WriteLine("Hello");
```

➢ รันโปรแกรมและบันทึกผล
<img width="852" alt="Screenshot 2024-03-23 205744" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/b56bc04c-7df4-40a0-afc4-0a89ebdfff7b">


👉 แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

```csharp
Console.Write("Hello, ");
Console.WriteLine("World!");
```

➢ รันโปรแกรมและบันทึกผล

<img width="870" alt="Screenshot 2024-03-23 205936" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/38298cf3-f4f4-4130-aa1f-118c6bc0bebd">

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
'Hello และ World อยู่ในบรรทัดเดียวกัน'

❔ จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
'Console.Write()จะแสดงคำให้อยู่ในบรรทัดเดียวกัน  แต่ Console.WriteLine()จะเว้นบรรทัด'

## [4. จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()](./Lab-01-part-4.md)
