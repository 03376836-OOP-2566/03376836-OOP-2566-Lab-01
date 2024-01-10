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
![2 1](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/139803cc-bd02-43bd-81e3-771e2ce4ad76)
`แสดงhelloในบรรทัดเดียวกัน`


### 2.2 การใช้เมดธอด Console.Write() ร่วมกับ  `Environment.NewLine`

`Environment.NewLine` เป็นค่าคงที่ที่ถูกนิยามในภาษา C# เพื่อใช้สำหรับการส่งอักขระขึ้นบรรทัดใหม่ไปยัง console

👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello" + Environment.NewLine);
Console.Write("Hello" + Environment.NewLine);
```

➢ รันโปรแกรมและบันทึกผล


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
![2 2](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/546f6656-38d2-40e5-9d86-5fbeac82f5e3)
`แสดงhelloแบบเว้นบรรทัด`



## 3. เมดธอด Console.WriteLine()

`Console.WriteLine()` เป็นคำสั่งที่เทียบเท่ากับการใช้  `Console.Write` ร่วมกับ  `Environment.NewLine` ทำให้ประหยัดเวลาในการเขียนโปรแกรม
👉 แก้โปรแกรมในเมดธอด Main() ให้เป็นดังต่อไปนี้

```csharp
Console.WriteLine("Hello");
```

➢ รันโปรแกรมและบันทึกผล
![3 1](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/f22a96e0-4c11-4587-a012-3487f34631bc)



👉 แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

```csharp
Console.Write("Hello, ");
Console.WriteLine("World!");
```

➢ รันโปรแกรมและบันทึกผล
![3 2](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/226c42fd-3608-406a-a3e9-30cd144d2350)

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
`Hello และ World อยู่ในบรรทัดเดียววัน`


❔ จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
'Console.Write()จะแสดงคำให้อยู่ในบรรทัดเดียวกัน  แต่ Console.WriteLine()จะเว้นบรรทัด'

## [4. จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()](./Lab-01-part-4.md)
