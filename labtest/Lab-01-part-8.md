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
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/082a53e8-11a7-4114-934e-49f1776676c9)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/53066f80-a551-4ba8-bfea-22d338890e78)
``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);

```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/077a02fe-fe26-4d60-95a7-121f6cae4173)
``` csharp
3. Console.WriteLine("Hello " + "World");
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/2d0abbbc-30b5-4d51-b291-8240adaa346d)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/94343299-6030-466f-9ea1-e8f6e7890cee)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/941ee973-f853-4e98-a3db-b4c274586387)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/bab110cc-04cb-4ee6-b1c0-fb151667df6c)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/bd9e1c26-7b91-4989-9562-bd83528d32ea)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/3d7f560a-722b-40d9-9070-9f89e5f4f904)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/4a2e67ff-18fd-4601-b145-403b588a0deb)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/f6af2fa1-20d2-4ca8-baab-0f241ad9eb71)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/146297c8-cf6b-40b2-bdba-9191c2f94f7e)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/327618c2-ea0e-498b-9ce3-0c5f17c4d2d6)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/44f013ee-286f-468a-b639-ad55fc5592b6)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/995f6569-7de7-4787-aef4-4fc0b6e4d271)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/ecf0fd14-d755-47c7-8b23-dfbd90e1b3c5)


## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
