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

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/85415f9a-852c-46c2-b62b-18ffdecfc13c)

## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/55247e37-05d4-4777-9048-146823252157)

``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/e650ef5e-260a-47a6-b4ae-f90129ec8588)

``` csharp
3. Console.WriteLine("Hello " + "World");
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/fde1db25-6aab-4c3e-9c1f-08c55b8b094a)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/2876e436-7519-4b2d-8098-5610232fad7d)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/cdca2663-c185-4990-b96b-73408ec5aed9)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/af44da94-8722-4766-a821-c559ed69717c)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/1733b96d-eca7-4675-8188-05ca97e30537)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/cf86e88f-8a9d-4626-bf33-0fd5e92d90df)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/cdede53b-df85-4613-8af4-8badb732369c)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/dd5f6db9-de80-4030-bcc2-9709eaa532c6)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/ad7aea22-4f58-4d9d-b1f9-f42e4130f1be)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/f28465e4-9c3c-4c57-a6d2-edcca260eb3b)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/637c37b3-3bdf-46d2-8c5a-3361febf8fb0)

``` csharp
14. 
```int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/a8c47477-6ed3-4f25-82c1-9ad2fccef463)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```

![image](https://github.com/likunzz/03376836-OOP-2566-Lab-01/assets/144196696/d50660ba-42c8-4bb3-8475-61236ef20f32)


## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
