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
![6 1](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/bf93ce83-79d4-46b5-83f7-9f9107a3ddc5)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![6 2](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/b167a8b6-a3ec-45be-9cd9-de0641a35b98)

``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
![6 3](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/ba6ae179-9b7e-4ea8-840b-c61f25efed8c)

``` csharp
3. Console.WriteLine("Hello " + "World");
```
![6 4](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/b8bf7116-0658-408c-b13d-0e743ca366c6)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
![6 5](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/81b30b6d-a384-42c7-85a8-77d8677ab5ef)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
![6 6](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/26399bb9-d2c5-4d2d-8cd4-4f66f60395ad)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
![6 7](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/c3f3fea6-ef8c-42ff-92f7-b13b502235f6)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![6 8](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/fe7fecb2-8413-4256-b701-2f50ab3a9776)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
![6 9](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/ac84259f-bdc1-4ac1-8862-ca3ef7401a1b)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
![6 10](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/d97020a1-c64b-4381-86bc-81ac4ac59b66)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
![6 11](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/ad81ea6f-1dd5-4ec0-ab99-e6a0163e5db9)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![6 12](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/44a3412e-f2ad-43cb-b86b-bb6f809b5a00)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
![6 13](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/0f292cc7-61e6-4b4b-b71e-8c97b080ab60)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
![6 14](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/7327c530-512e-4ec1-95f1-0c352554a216)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![6 15](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/602bfe29-d1a2-48a7-be75-938b0f5332bf)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```
![6 16](https://github.com/VisawaPRO/03376836-OOP-2566-Lab-01/assets/144195555/224dbd06-7202-4d9d-8bd0-700aec7ff89a)



## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
