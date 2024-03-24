# Lab-01 Part 2~3 คำสั่ง Console.Write() และ Console.WriteLine()

## 2. การใช้เมดธอด Console.Write()

### 2.1 การใช้เมดธอด Console.Write()
👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello");
Console.Write("Hello");
```

➢ รันโปรแกรมและบันทึกผล
![ข้อ 2 1](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/1795b751-63ef-4afa-b988-e681acebf685)


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
![ข้อ 2 2](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/f38a2caf-e7ed-4e96-b4c1-7cf5a7cda805)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
#### เป็นไปตามที่คิดไว้ เพราะใช้คำสั่งให้โปรแกรมขึ้นบรรทัดใหม่จึงได้ผลอยู่คนละบรรทัดกัน

## 3. เมดธอด Console.WriteLine()

`Console.WriteLine()` เป็นคำสั่งที่เทียบเท่ากับการใช้  `Console.Write` ร่วมกับ  `Environment.NewLine` ทำให้ประหยัดเวลาในการเขียนโปรแกรม
👉 แก้โปรแกรมในเมดธอด Main() ให้เป็นดังต่อไปนี้

```csharp
Console.WriteLine("Hello");
```

➢ รันโปรแกรมและบันทึกผล
![ข้อ 3 1](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/11a7d5ef-d03c-4fa5-8cf3-e2c9eb8a9cbc)


👉 แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

```csharp
Console.Write("Hello, ");
Console.WriteLine("World!");
```

➢ รันโปรแกรมและบันทึกผล
![ข้อ 3 2](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/1c3f3dce-411f-4033-9469-8d9ba6451b21)

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
#### เป็นไปตามที่คิด เพราะได้ผลติดกัน Console.Write ข้อมูลต่อท้ายกับข้อมูลแสดงล่าสุดในบรรทัดเดียวกัน

❔ จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
#### Console.Write() : ต้องการแสดงผลข้อความหลายบรรทัดติดต่อกันโดยไม่ขึ้นบรรทัดใหม่
#### Console.WriteLine() : แสดงผลข้อความแต่ละบรรทัดแยกกันโดยขึ้นบรรทัดใหม่

## [4. จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()](./Lab-01-part-4.md)
