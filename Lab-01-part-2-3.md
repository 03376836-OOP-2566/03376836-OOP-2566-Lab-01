# Lab-01 Part 2~3 คำสั่ง Console.Write() และ Console.WriteLine()

## 2. การใช้เมดธอด Console.Write()

### 2.1 การใช้เมดธอด Console.Write()
👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello");
Console.Write("Hello");
```

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/307edb4a-c15e-4238-9c11-be8a18693ef3)



❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย

        ผลการทดลองเป็นไปตามที่คิดที่จะแสดงคำว่า HELLO ออกมาสองครั้ง

### 2.2 การใช้เมดธอด Console.Write() ร่วมกับ  `Environment.NewLine`

`Environment.NewLine` เป็นค่าคงที่ที่ถูกนิยามในภาษา C# เพื่อใช้สำหรับการส่งอักขระขึ้นบรรทัดใหม่ไปยัง console

👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello" + Environment.NewLine);
Console.Write("Hello" + Environment.NewLine);
```

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/317e353a-65fe-49a1-a77e-14cc18180325)



❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย

      เป็นที่ได้ตามที่คาดคิดไว้ว่า Hello จะแบ่งบรรทัดเพราะคำสั่ง Environment.Newline


## 3. เมดธอด Console.WriteLine()

`Console.WriteLine()` เป็นคำสั่งที่เทียบเท่ากับการใช้  `Console.Write` ร่วมกับ  `Environment.NewLine` ทำให้ประหยัดเวลาในการเขียนโปรแกรม
👉 แก้โปรแกรมในเมดธอด Main() ให้เป็นดังต่อไปนี้

```csharp
Console.WriteLine("Hello");
```

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/0da20bc1-1007-4506-a1b6-d1d267d37cf2)



👉 แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

```csharp
Console.Write("Hello, ");
Console.WriteLine("World!");
```

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/a890066b-e884-4ae3-b765-36b34ca4f4b6)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย

ไม่เป็นไปดั่งที่คิดเพราะตอนแรกคิดว่าโค้ดจะแบ่งบรรทัดเพราะคำสั่งwriteline


❔ จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()

Consolewrite จะเป็นการรวมคำสั่งไว้ในบรรทัดเดียวกัน แต่ Console.WriteLine จะเป็นคำสั่งเว้นบรรทัด


## [4. จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()](./Lab-01-part-4.md)
