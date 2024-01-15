# Lab-01 Part 2~3 คำสั่ง Console.Write() และ Console.WriteLine()

## 2. การใช้เมดธอด Console.Write()

### 2.1 การใช้เมดธอด Console.Write()
👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello");
Console.Write("Hello");
```

➢ รันโปรแกรมและบันทึกผล
![Screenshot 2024-01-15 215156](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/dc96dfb1-7a3c-4d7c-a616-03cd8eda6b68)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
#### เป็นไปตามที่คิด เพราะคำสั่ง Console.Write 2 รอบ แสดงผลออกมาได้ข้อความติดกัน

### 2.2 การใช้เมดธอด Console.Write() ร่วมกับ  `Environment.NewLine`

`Environment.NewLine` เป็นค่าคงที่ที่ถูกนิยามในภาษา C# เพื่อใช้สำหรับการส่งอักขระขึ้นบรรทัดใหม่ไปยัง console

👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello" + Environment.NewLine);
Console.Write("Hello" + Environment.NewLine);
```

➢ รันโปรแกรมและบันทึกผล
![Screenshot 2024-01-15 215227](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/04debd4b-a64e-48c8-8a43-9ce16b64659e)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
#### เป็นไปตามที่คิดไว้ เพราะใช้คำสั่งให้โปรแกรมขึ้นบรรทัดใหม่จึงได้ผลอยู่คนละบรรทัดกัน

## 3. เมดธอด Console.WriteLine()

`Console.WriteLine()` เป็นคำสั่งที่เทียบเท่ากับการใช้  `Console.Write` ร่วมกับ  `Environment.NewLine` ทำให้ประหยัดเวลาในการเขียนโปรแกรม
👉 แก้โปรแกรมในเมดธอด Main() ให้เป็นดังต่อไปนี้

```csharp
Console.WriteLine("Hello");
```

➢ รันโปรแกรมและบันทึกผล
![Screenshot 2024-01-15 215256](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/ab339810-bef0-489b-ad2c-c3af00ff4f3b)


👉 แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

```csharp
Console.Write("Hello, ");
Console.WriteLine("World!");
```

➢ รันโปรแกรมและบันทึกผล
![Screenshot 2024-01-15 215323](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/eacd2382-25fa-440c-a0db-0068cd44bfa2)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
#### เป็นไปตามที่คิด เพราะได้ผลติดกัน Console.Write ข้อมูลต่อท้ายกับข้อมูลแสดงล่าสุดในบรรทัดเดียวกัน

❔ จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
#### Console.Write() : ต้องการแสดงผลข้อความหลายบรรทัดติดต่อกันโดยไม่ขึ้นบรรทัดใหม่
#### Console.WriteLine() : แสดงผลข้อความแต่ละบรรทัดแยกกันโดยขึ้นบรรทัดใหม่

## [4. จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()](./Lab-01-part-4.md)
