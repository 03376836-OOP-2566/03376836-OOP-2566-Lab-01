# Lab-01 Part 2~3 คำสั่ง Console.Write() และ Console.WriteLine()

## 2. การใช้เมดธอด Console.Write()

### 2.1 การใช้เมดธอด Console.Write()
👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello");
Console.Write("Hello");
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/6702a87b-3f6a-437c-808e-279826c05819)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
 ```เป็นอย่างที่คิด คือเเสดง Hello 2 บรรทัดจากคำสั่งดังกล่าว ```

### 2.2 การใช้เมดธอด Console.Write() ร่วมกับ  `Environment.NewLine`

`Environment.NewLine` เป็นค่าคงที่ที่ถูกนิยามในภาษา C# เพื่อใช้สำหรับการส่งอักขระขึ้นบรรทัดใหม่ไปยัง console

👉 แก้ไขโปรแกรม ให้เป็นดังด้านล่างนี้

```csharp
Console.Write("Hello" + Environment.NewLine);
Console.Write("Hello" + Environment.NewLine);
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/02651eef-fb2f-4025-8f74-ab159236a629)


❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
``` เป็นอย่างที่คิด คือเเสดง Hello 2 บรรทัด เพราะไม่มี่อักขระที่จะขึ้นบรรทัดใหม่ไปยัง console```

## 3. เมดธอด Console.WriteLine()

`Console.WriteLine()` เป็นคำสั่งที่เทียบเท่ากับการใช้  `Console.Write` ร่วมกับ  `Environment.NewLine` ทำให้ประหยัดเวลาในการเขียนโปรแกรม
👉 แก้โปรแกรมในเมดธอด Main() ให้เป็นดังต่อไปนี้

```csharp
Console.WriteLine("Hello");
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/cf2b8b72-211b-401b-a41b-da75f81d8155)


👉 แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

```csharp
Console.Write("Hello, ");
Console.WriteLine("World!");
```

➢ รันโปรแกรมและบันทึกผล
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/f0ab8350-d75a-4c99-831d-29b33a0047c6)

❔ ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร จงอธิบาย
  ``` เป็นอย่างที่คิด เพราะ จากคำสั่งจะทำให้ข้อความต่อกันดังคำอธิบาย ```
❔ จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
  ``` คำสั่ง Console.Write() และ Console.WriteLine() เป็นคำสั่งที่ใช้ในภาษา C# เพื่อแสดงผลข้อความในหน้าคอนโซล (console). ความแตกต่างระหว่างทั้งสองคำสั่งคือ:
   Console.Write():
ใช้เพื่อแสดงข้อความหรือข้อมูลบนหน้าคอนโซลโดยไม่ขึ้นบรรทัดใหม่หลังจากข้อความนั้น.
ไม่ทำการเพิ่มบรรทัดใหม่หลังจากข้อความที่ถูกแสดง.
   Console.WriteLine():
ใช้เพื่อแสดงข้อความหรือข้อมูลบนหน้าคอนโซลและทำการขึ้นบรรทัดใหม่หลังจากข้อความนั้น.
เพิ่มบรรทัดใหม่หลังจากข้อความที่ถูกแสดง.
```
## [4. จำนวนของอาร์กิวเมนต์ในคำสั่ง Console.WriteLine()](./Lab-01-part-4.md)