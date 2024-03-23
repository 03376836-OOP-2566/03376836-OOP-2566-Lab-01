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
## ![Screenshot 2024-03-23 204614](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/094f6cbc-a483-44c3-b825-8d11178151d4)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
## ![Screenshot 2024-03-23 204958](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/d0479dfe-1e40-4860-b128-1aa92c4af897)


``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
## ![Screenshot 2024-03-23 205017](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/e63c20d5-2dcc-4978-b9a6-f246dd46283b)


``` csharp
3. Console.WriteLine("Hello " + "World");
```
## ![Screenshot 2024-03-23 205033](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/e5347338-9099-4efc-9f56-d8fbd0ba286a)


``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
## ![Screenshot 2024-03-23 205050](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/317ef25c-7358-4634-8399-1b007beb61ae)


``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
## ![Screenshot 2024-03-23 205108](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/594efd40-196b-4094-9b49-2f81c67c4133)


``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
## ![Screenshot 2024-03-23 205128](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/e597c858-a968-4f2f-a323-3d2def65d336)


``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
## ![Screenshot 2024-03-23 205150](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/24dae867-d8d9-4716-aa90-5cfe2b505c14)


``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
## ![Screenshot 2024-03-23 205213](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/314f2498-2eb3-46fd-8802-3216df89625b)


``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
## ![Screenshot 2024-03-23 205230](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/a1902a30-d114-4e2b-8d96-a8830c26aebc)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
## ![Screenshot 2024-03-23 205248](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/1e428d78-81d2-4f5e-befa-733eb630a783)


``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
## ![Screenshot 2024-03-23 205335](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/136d980f-6c76-4f28-926a-aeeb295e7c9f)


``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
## ![Screenshot 2024-03-23 205404](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/d2c8ede9-8566-4f22-b851-2502cf858991)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
## ![Screenshot 2024-03-23 205433](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/e8b230f4-40bf-4290-b258-27ce10b008bc)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
## ![Screenshot 2024-03-23 205508](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/1c2d07fa-a262-4fc1-815d-23df6f06c0a8)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```
## ![Screenshot 2024-03-23 205524](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/c5190ef2-f69d-49fa-ba3b-761e02a9d99a)



## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
