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
![ข้อ 8](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/dc0c65ab-80f1-403b-b2b8-03bf4e579bbf)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![แบบฝึกหัด 1](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/2e30986e-6acb-49d7-ae76-551344dd4954)

``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
![แบบฝึกหัด 2](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/6bcd8df7-ed5a-4583-a376-ce9a45e67815)

``` csharp
3. Console.WriteLine("Hello " + "World");
```
![แบบฝึกหัด 3](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/ec8b70e5-5d3d-4ae2-aadf-f32a59c0ebbb)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
![แบบฝึกหัด 4](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/1ffd9bb4-f710-4864-ada7-3f40264ad1fe)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
![แบบฝึกหัด 5](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/641477ba-4f8f-4e10-95bf-1fa59ffa30e3)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
![แบบฝึกหัด 6](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/6f5c3428-eba4-4ed6-9ec4-6dd246c6426a)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![แบบฝึกหัด 7](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/8726ea26-b599-4610-95dc-0c8d580265a1)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
![แบบฝึกหัด 8](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/8874c6e2-6a20-4dad-8f4b-b11f04ad88a6)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
![แบบฝึกหัด 9](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/aff394eb-8310-4561-b6cf-3f58a40b3537)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
![แบบฝึกหัด 10](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/6deccbee-ddb3-4798-8324-ba12637b3a99)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![แบบฝึกหัด 11](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/d8077c34-2ba2-4f00-80b9-e52234622a2f)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
![แบบฝึกหัด 12](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/5943b013-6219-4b08-a2de-eec2bb0e9c06)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
![แบบฝึกหัด 13](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/2a2ebf11-8623-4796-892d-98f976d86979)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![แบบฝึกหัด 14](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/0da19853-0d67-480f-bacb-e85fc76947bc)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```
![แบบฝึกหัด 15](https://github.com/65030179179Pattarapon/03376836-OOP-2566-Lab-01/assets/144198506/8d8e7342-bdfd-4280-aa0c-98635b152ae3)


## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
