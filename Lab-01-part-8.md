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

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/940dfd81-c1bc-4178-8eee-a111035c5eea)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/4b81ed34-d0ef-44bc-8826-ccfd376d20fe)

``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/ca2d28cc-b7dd-4c89-ba59-c1eb477dc453)

``` csharp
3. Console.WriteLine("Hello " + "World");
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/ff57cd42-5083-4122-a84e-c4bcbaf3305f)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/1a96ea7b-6d71-4bb2-9cf8-a684673a4e92)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/f7984e94-b1e0-43b5-b3ae-c8eba65f8451)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/d97908ae-9ae1-466e-abd3-ed533af7e235)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/934f0ca5-fb4b-41a2-93f3-7f707c457d21)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/c3d38458-e6da-4e9a-a949-ea3c2973e714)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/86c5a9b6-388b-4539-a62d-1e8f95e5ecea)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/3f85f18f-8a2e-49bb-bbed-b793b568ac89)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/1edab3f7-90bc-414b-87f1-5c29e1e0af3c)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/9c1e1e63-4db7-4df9-bdec-debbf2c28d1e)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/4427f2a3-8222-4454-902e-3cd384eaaed0)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```

![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/238ef6c6-8cef-48ee-bbcf-074d222ed4a7)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```


![image](https://github.com/Siriratda/03376836-OOP-2566-Lab-01/assets/144195995/abbdd1ce-6822-4f66-a5c1-82b511229b79)



## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
