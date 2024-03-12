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

![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/bd2b3a68-d4b1-4324-ad62-1ec10e021f17)

 
👷 จากจ้อ 14 ให้เขียนโปรแกรมเพื่อสร้างตารางความจริงของลอจิกดังต่อไปนี้

1. `AND`
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/bc97cb4d-5b29-4028-816a-9dfd8a370ae4)
2. `OR`
![294659260-1530a1bf-4e11-4dcb-a7fa-95bfc5af0cb2](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/45376cc9-bc11-48b1-bc12-5dcdddb7ea61)
3. `NOT`
![294659265-810f3d9f-d055-4e7b-9da6-e289e7bed275](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/b887735a-99ea-450d-abe8-87bfdc093404)
4. `NAND`
![294659272-ca563eaa-b302-47b0-b3a4-b77924f5bd10](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/13ebefac-ff00-4297-b573-461541eb5a72)
5. `NOR
 ![294659286-519652d3-b33e-42a1-bede-5ca7fd229095](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/be0ef155-ed04-4bce-81ea-fcf41b4ff13c)
6. `Exclusive OR`
![294659296-05712c42-552a-4ab0-b6b4-1c4a13ebcfbd](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/ffc399fa-1443-4829-b952-84ebce0d7488)


## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
