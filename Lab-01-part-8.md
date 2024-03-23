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
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/b6a9117f-e9ed-4445-871f-eae8bd35392d)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/aec73d87-7937-48b1-87b3-86e8eae95b22)

``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/fa3284cb-0e41-4645-831c-c4d702b0b479)

``` csharp
3. Console.WriteLine("Hello " + "World");
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/4df8e5fd-2112-46fa-bf78-cad556851edf)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/93fc94d1-1b65-4e76-b897-0e1b1c96947c)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/d1ea0e8b-bc1f-46a7-9014-1b8501fcba45)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/c64e5038-3db1-4e0f-826a-598025f4c76b)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/603d6e5d-2020-4909-ace8-79e9edaa8c44)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/2b4d2ce5-a3f1-42d1-89cc-73cc2100011b)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/9dd2c080-b202-4243-8e8d-ca311d482c83)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/3a87e097-f30e-4e02-8a8b-8a0093767396)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/7bb85edc-649c-4889-a8e9-f80c9e0ceb34)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/aa353595-b79d-4493-a09e-2c04ee94bc9c)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/5581bb38-2893-4da1-ab01-b6ee8c70bd79)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/cc4de5ea-4abf-42f8-9b06-e7cb0a417c34)


``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```
![image](https://github.com/chatladawongkanyon/03376836-OOP-2566-Lab-01/assets/144195963/f9193ee3-bd6f-40a7-b4f7-c3ac3819f397)


## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
