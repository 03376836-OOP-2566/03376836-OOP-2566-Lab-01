# Lab-01 Part 2~3 คำสั่ง Console.Write() และ Console.WriteLine()

## 2. การใช้เมดธอด Console.Write()

### 2.1 การใช้เมดธอด Console.Write()
👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello");
Console.Write("Hello");
```

➢ รันโปรแกรมและบันทึกผล
![Screenshot 2024-03-25 003717](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/55c4395a-23a2-4a82-9742-3934991448d2)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
yes

### 2.2 การใช้เมดธอด Console.Write() ร่วมกับ  `Environment.NewLine`

`Environment.NewLine` เป็นค่าคงที่ที่ถูกนิยามในภาษา C# เพื่อใช้สำหรับการส่งอักขระขึ้นบรรทัดใหม่ไปยัง console

👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello" + Environment.NewLine);
Console.Write("Hello" + Environment.NewLine);
```

➢ รันโปรแกรมและบันทึกผล
![Screenshot 2024-03-25 003834](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/957963bc-33b9-422c-a598-5264e29fc2ad)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
yes

## 3. เมดธอด Console.WriteLine()

`Console.WriteLine()` เป็นคำสั่งที่เทียบเท่ากับการใช้  `Console.Write` ร่วมกับ  `Environment.NewLine` ทำให้ประหยัดเวลาในการเขียนโปรแกรม
👉 แก้โปรแกรมในเมดธอด Main() ให้เป็นดังต่อไปนี้

```csharp
Console.WriteLine("Hello");
```

➢ รันโปรแกรมและบันทึกผล
![Screenshot 2024-03-25 003931](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/615ebe0b-4416-486a-b6fa-1595a8c1c2d2)


👉 แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

```csharp
Console.Write("Hello, ");
Console.WriteLine("World!");
```

➢ รันโปรแกรมและบันทึกผล
![Screenshot 2024-03-25 004012](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/665a15c8-02ec-44d7-b0c3-39313f84c997)

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
yes

❔ จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
Console.WriteLine() จะแสดงผลข้อความหรือข้อมูลที่ระบุแล้วขึ้นบรรทัดใหม่
Console.Write() โปรแกรมจะแสดงผลข้อความหรือข้อมูลที่ระบุโดยไม่ขึ้นบรรทัดใหม่

## [4. จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()](./Lab-01-part-4.md)
