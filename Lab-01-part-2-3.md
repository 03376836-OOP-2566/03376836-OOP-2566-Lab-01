# Lab-01 Part 2~3 คำสั่ง Console.Write() และ Console.WriteLine()

## 2. การใช้เมดธอด Console.Write()

### 2.1 การใช้เมดธอด Console.Write()
👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello");
Console.Write("Hello");
```

➢ รันโปรแกรมและบันทึกผล
## ![Screenshot 2024-03-23 201045](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/99e76944-66cc-4b5b-b4df-f801b82b04b3)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
#### Anser Helloติดกันครับ
### 2.2 การใช้เมดธอด Console.Write() ร่วมกับ  `Environment.NewLine`

`Environment.NewLine` เป็นค่าคงที่ที่ถูกนิยามในภาษา C# เพื่อใช้สำหรับการส่งอักขระขึ้นบรรทัดใหม่ไปยัง console

👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello" + Environment.NewLine);
Console.Write("Hello" + Environment.NewLine);
```

➢ รันโปรแกรมและบันทึกผล
## ![Screenshot 2024-03-23 201111](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/2a829700-68a2-4dcf-be47-c0b293162d28)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
#### Anser Helloจะลงมาอยู่ด้านล่างครับ

## 3. เมดธอด Console.WriteLine()

`Console.WriteLine()` เป็นคำสั่งที่เทียบเท่ากับการใช้  `Console.Write` ร่วมกับ  `Environment.NewLine` ทำให้ประหยัดเวลาในการเขียนโปรแกรม
👉 แก้โปรแกรมในเมดธอด Main() ให้เป็นดังต่อไปนี้

```csharp
Console.WriteLine("Hello");
```

➢ รันโปรแกรมและบันทึกผล
## ![Screenshot 2024-03-23 201141](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/3f594838-aa4b-415d-aa40-ef706375d10b)


👉 แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

```csharp
Console.Write("Hello, ");
Console.WriteLine("World!");
```

➢ รันโปรแกรมและบันทึกผล
## ![Screenshot 2024-03-23 201202](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/48ddc870-6442-451c-ac01-bed711044f16)

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
#### เป็นอย่างที่คิดครับเพราะเคยเรียนเรื่อง Console.Write และ Console.WriteLine จา่กอาจารย์แล้วครับ

❔ จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
####  Console.Write(): ไม่ขึ้นบรรทัดใหม่หลังจากแสดงผลลัพธ์ ข้อความจะแสดงต่อบนบรรทัดเดียวกัน
####  Console.WriteLine(): ขึ้นบรรทัดใหม่หลังจากแสดงผลลัพธ์ ข้อความจะแสดงบนบรรทัดใหม่

## [4. จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()](./Lab-01-part-4.md)
