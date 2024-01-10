# Lab-01 การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ

ตัวแปรชนิด boolean มักจะถูกใช้เป็นที่เก็บผลที่เกิดจากการดำเนินการทางตรรกะ เช่น AND, OR, NOT เป็นต้น ซึ่งการดำเนินการทางตรรกะจะมีตารางความจริง เป็นตัวบอกผลในการดำเนินการของตัวดำเนินการต่างๆ ดังตัวย่าง

### ตัวดำเนินการ AND

Y = A AND B

| A | B | Y |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

### ตัวดำเนินการ OR

Y = A OR B

| A | B | Y |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

### ตัวดำเนินการ NOT

Y = NOT A

| A | Y |
|--|--|
| 0 | 1 |
| 1 | 0 |

ตัวดำเนินการในภาษา C#
ใช้เครื่องหมายต่างๆ ดังต่อไปนี้

| การดำเนินการ | เครื่องหมาย |
|------------|-----------|
| Logical AND | & |
| Logical XOR | ^ |
| Logical OR | \| |

## 14. การเขียนโปรแกรมด้วยตัวดำเนินการทางตรรกะ

ตัวอย่างภาษา C# ต่อไปนี้เป็นการพิมพ์ตารางความจริงออกทางหน้าจอ
👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
bool A, B,Y;
Console.WriteLine("      Y = A AND B");
Console.WriteLine("-----------------------");
Console.WriteLine("   A      B\t|  Y");
Console.WriteLine("-----------------------");
A = false; B = false; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A,B,Y);
A = false; B = true; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
A = true; B = false; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
A = true; B = true; Y = A & B;
Console.WriteLine(" {0}\t{1}\t| {2}", A, B, Y);
Console.WriteLine("-----------------------");
```

➢ รันโปรแกรมและบันทึกผล

 
👷 จากจ้อ 14 ให้เขียนโปรแกรมเพื่อสร้างตารางความจริงของลอจิกดังต่อไปนี้

1. `AND`![and](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/91139c3f-ca9b-4030-8339-bc6fa4666761)

2. `OR`![or](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/808c7387-c13e-45c9-82c0-eff5b84aa7fa)

3. `NOT`![not](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/d1e85590-a277-4974-9e9c-34a2ea794a3a)

4. `NAND`![NAND](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/6130bae8-d021-4cac-b95d-f325d3454464)

5. `NOR`![nor](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/95849f7d-b4c9-4444-84c0-22b564adcbee)

6. `Exclusive OR`![xor](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/b3336554-1102-44e0-9a50-3be645afc587)



## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
