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
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/b8bd3a1f-e940-4966-a6f5-265499eb291c)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/dac50e3c-61db-4da8-aa99-da91991cb6a9)

``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/12f6abbb-4910-40d8-ac93-ccdcdcd8a169)

``` csharp
3. Console.WriteLine("Hello " + "World");
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/f4430dee-8e9c-417f-9b3b-671b8b149a85)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/7068d46d-4245-46c4-a262-199afd609d6b)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/345cf414-5cec-49eb-b1a1-868f4f1ad1fb)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/2f4d9625-17eb-4672-9f17-0fffa4582e9d)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/a3380627-ed64-4376-a496-ddc140deb6cf)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/35affc80-5f59-4628-9694-3b62eab69442)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/2e457615-f26a-4f4e-a933-2a3f0da77a8d)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/b086b6c6-93b0-41e6-af99-735a085c2c0a)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/82c62009-92da-46d6-b091-166e7b4017e9)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/2910b406-4c00-4a79-a48f-9b481cf48d0c)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/212aea4f-34a9-47ad-bd7d-4c3beed568b7)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/7758bfc4-c58d-412f-8c03-0cd4b5c56ee9)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```
![ภาพ](https://github.com/AnchisaPhetnoi/03376836-OOP-2566-Lab-01/assets/144197034/704de05d-ed50-43d2-9274-7b14ed64071f)


## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
