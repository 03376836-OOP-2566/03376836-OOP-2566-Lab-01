# Lab-01  Part 8  การกำหนดรูปแบบพร้อมความกว้างของทศนิยมของอาร์กิวเมนต์

👉 แก้โปรแกรมตามรูปด้านล่างนี้
```csharp
const double i = 123.456789d;
Console.WriteLine("{0:F1}", i);
Console.WriteLine("{0:F2}", i);
Console.WriteLine("{0:F3}", i);
Console.WriteLine("{0:F4}", i);
Console.WriteLine("{0:F5}", i);
```
➢ รันโปรแกรมและบันทึกผล

![Screenshot 2024-01-15 215804](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/10a49034-b1d3-440d-8cfc-4b12692a35dc)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![Screenshot 2024-01-15 215844](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/d307ad14-1ac2-4261-a804-9084a573754e)


``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```

![Screenshot 2024-01-15 215909](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/3cec1ded-fb0f-4411-8a45-616c378e0b65)


``` csharp
3. Console.WriteLine("Hello " + "World");
```

![Screenshot 2024-01-15 215939](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/e3dd233c-36bd-4cc6-a400-7536f42ce3df)


``` csharp
4. Console.WriteLine("Here comes a slash \\");
```

![Screenshot 2024-01-15 220013](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/12fe3790-7cc9-46ca-898c-50c2cf0a6bc1)


``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```

![Screenshot 2024-01-15 220057](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/286c9504-1467-46e1-b464-aa63afa0a81f)


``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```

![Screenshot 2024-01-15 220130](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/cf61e96a-be3c-448f-a570-579e60d98d9a)


``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![Screenshot 2024-01-15 220156](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/2c30e71e-ec4a-46be-a58f-3ffbe4cff28e)


``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```

![Screenshot 2024-01-15 220224](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/f15cead8-bd53-4138-aae7-68038d6dcbbb)


``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```

![Screenshot 2024-01-15 220249](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/9e14cf95-8523-401a-a416-173872c92077)


``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```

![Screenshot 2024-01-15 220434](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/362a0ad1-c85f-4dc0-a4f8-c373914ef517)


``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![Screenshot 2024-01-15 220502](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/aed0e30a-162f-45e6-84f2-841507e114b4)



``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```

![Screenshot 2024-01-15 220532](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/2c7d76f7-73ff-4527-b89f-fea47c4a8aa0)


``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```

![Screenshot 2024-01-15 220605](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/bb73ab77-6ccf-4e03-aaae-de3fc7bc357a)


``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![Screenshot 2024-01-15 220638](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/e5998063-b7f2-45d6-8a7d-538d9c81aec4)



``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```

![Screenshot 2024-01-15 220709](https://github.com/KanyakornPuengmon/03376836-OOP-2566-Lab-01/assets/144195697/202d523a-c6ca-4312-9a0e-7eff97443003)




## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
