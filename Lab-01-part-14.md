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
![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/a96ab66d-39f4-439e-9c18-e944dc9c81af)


 
👷 จากจ้อ 14 ให้เขียนโปรแกรมเพื่อสร้างตารางความจริงของลอจิกดังต่อไปนี้

1. `AND`
    ![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/5b9aa8cf-7db4-4347-b6ed-805a65bd511e)

2. `OR`
   ![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/c6ac3a99-2915-49aa-a2ed-f3b6aaa34835)


3. `NOT`
   ![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/4d5c47bb-42ff-490a-84bc-492ad97f722f)

   
4. `NAND`
    ![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/e37db4f6-c069-4e05-afa9-3a1f2ab746ff)

  
6. `NOR`
   ![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/e738e617-ae52-4a5c-912e-6446e102b0e6)

8. `Exclusive OR`
   ![image](https://github.com/ThanchiraCharakhon099/03376836-OOP-2566-Lab-01/assets/144195708/cc29db72-0c44-4219-8c67-4c398a8d238b)



## [ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)](./Lab-01-part-15.md)
