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

![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/1d230bc1-2699-4148-965c-a5dad9bc5dd2)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/82dd5d5e-cdc0-47ab-b7e3-84235e829d38)


``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);

![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/a3f69dfc-adf3-4f6a-bcfe-75522fd5a17c)

```
``` csharp
3. Console.WriteLine("Hello " + "World");
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/be707b82-61e5-4c0f-bedb-6c9d90a0c44f)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/102dc623-a9af-4ab1-8025-f53c86ac8899)


``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/0280da43-a6f0-4e90-aefe-aee8b13dfd2c)


``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/9dd4bdc0-fa84-4f59-b08d-a0df8b7ab003)


``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/4d0f8df8-0306-4fcd-b569-82d87dd20883)


``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/6d229af8-ca03-459a-ab4f-1ea3cb3894e1)


``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/f6824de0-56f8-4f24-be22-ab4393cd46e8)


``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/43f10f45-3185-41ba-88e6-dffc4324f91a)


``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/b691df5c-4243-499d-9fb9-fc7b6f508537)


``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/e16bd42e-1420-4a7f-b00d-1573ca7ff80d)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/c5d469c2-e672-4251-aa45-123a623ca0d9)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/14672b0b-da18-4bbd-9da1-f84a97e3b596)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```

![image](https://github.com/fulk2014/03376836-OOP-2566-Lab-01/assets/144195753/f81baee3-5527-4689-817c-bce4a0afd395)



## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
