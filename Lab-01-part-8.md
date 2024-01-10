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
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/b0452123-770c-4f84-943a-d7c8fa7e7441)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/ebce9326-9d77-4d64-82ee-2f26f2312f54)

``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/e64c877c-e428-4432-b3f8-9bc55584520f)

``` csharp
3. Console.WriteLine("Hello " + "World");
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/ec7ecdfe-cc98-4ffd-812b-0f6b66f4a451)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/3cb0151a-6217-4e5a-bbb2-98aa923b690a)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/98467d1e-2a21-4815-898d-b08716468d74)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/45f5bd6b-be4d-435e-a33f-088173b0131b)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/b31af628-1769-4305-a7a6-1109c8ce24ad)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/60930fa3-0a6d-4466-beeb-c8aa112729d9)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/4a301e86-88db-47f6-ac34-196558347093)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/d76a7d36-c21a-4668-9450-a987d4792cc9)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/494f2cef-8abb-4dce-930d-7f8fbae2e490)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/e8fe9e4f-2e14-4a9e-bd86-a46bf64e5864)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/11c51d04-5623-40ab-beca-24630bbe630f)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/203505d4-d83f-431b-82be-9dbf027bd553)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/c9597304-bafa-4647-9019-9bc5db89e0df)



## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
