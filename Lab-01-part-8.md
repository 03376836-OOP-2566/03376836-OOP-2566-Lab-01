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
![Screenshot 2024-03-25 005200](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/9fdaf1a3-79f0-411e-a372-b4fdcfec06cb)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![Screenshot 2024-03-25 005519](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/ad78231a-c2c7-4860-8f04-ed57e31f39ea)

``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
![Screenshot 2024-03-25 005548](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/1c285ab6-d9d1-43bc-ac47-7fc608b09e32)

``` csharp
3. Console.WriteLine("Hello " + "World");
```
![Screenshot 2024-03-25 005615](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/b54ca91d-8aee-4909-9c99-e2977d3cdf8f)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
![Screenshot 2024-03-25 005649](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/12b697c9-9fa3-4acd-a658-71c171ccc3a5)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
![Screenshot 2024-03-25 005714](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/289a8a97-c9cb-42d9-b888-951c07076bc4)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
![Screenshot 2024-03-25 005736](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/c0ad2166-a7ed-468c-8036-b563a5914f39)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![Screenshot 2024-03-25 005755](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/a4e24ede-8356-4490-825b-6d325f33ce53)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
![Screenshot 2024-03-25 005827](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/c3c419a5-85cd-4fbc-8ff1-688dae045249)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
![Screenshot 2024-03-25 005851](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/afec04a8-1366-445e-a1f5-8ea2377dcaf4)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
![Screenshot 2024-03-25 005929](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/a2521c31-9976-4137-9d58-dbfeb5458721)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![Screenshot 2024-03-25 005959](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/06033d63-512b-4a1e-9360-1454e843e40c)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
![Screenshot 2024-03-25 010037](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/d3b2adf0-14c4-42b0-aa20-efa571399236)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
![Screenshot 2024-03-25 010134](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/7ad28a0d-35c1-47bc-b080-02bef124856b)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![Screenshot 2024-03-25 010156](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/4eb1e732-26d5-441c-8d4f-08e80d5d3f4c)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```
![Screenshot 2024-03-25 010220](https://github.com/omelaweng/03376836-OOP-2566-Lab-01/assets/144561325/883eede8-017a-4d1f-a8a8-9db319ac93cb)


## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
