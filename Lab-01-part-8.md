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
![Screenshot 2024-01-18 141608](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/fc4e19c9-074f-4d50-bb3d-4eade8a26d91)


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![Screenshot 2024-01-18 141917](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/68f09cc0-0952-4ccf-ae81-73b65b9e408c)

``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
![Screenshot 2024-01-18 141940](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/61fa6758-8e58-4a16-9ee6-9a3f52b228bb)

``` csharp
3. Console.WriteLine("Hello " + "World");
```
![Screenshot 2024-01-18 141956](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/ed3e5802-2edb-467e-846b-057a56696fa0)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
![Screenshot 2024-01-18 142015](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/56183391-962b-4066-95c1-5c1fa2078df9)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
![Screenshot 2024-01-18 142031](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/491128f1-d2d5-4446-9e64-02637e06ae71)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
![Screenshot 2024-01-18 142049](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/7262bcdb-18ea-4e0d-9827-fce6fc28651e)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![Screenshot 2024-01-18 142108](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/bdaed9f3-b442-4f03-81ef-42153cdaf8e0)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
![Screenshot 2024-01-18 142247](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/8a327481-0e52-4215-812e-5dc7cfe532c5)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
![Screenshot 2024-01-18 142301](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/193934c0-55c1-49b7-a194-3973388daf9e)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
![Screenshot 2024-01-18 142313](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/19a51930-2c6d-47d5-a333-3f6284213607)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![Screenshot 2024-01-18 142325](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/eb60aea3-4778-49ad-8058-cd0036946380)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
![Screenshot 2024-01-18 142545](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/faa6abb2-4263-4d70-bcdf-491efbc4ed1b)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
![Screenshot 2024-01-18 142604](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/a33ae29d-e897-4553-ac21-dc94814ccc64)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![Screenshot 2024-01-18 142626](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/1cc799ba-39e7-465f-8676-04a6388e711b)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```

![Screenshot 2024-01-18 142655](https://github.com/Chaiyapa/03376836-OOP-2566-Lab-01/assets/144195729/2a466d94-ceba-4c05-8b00-12e2ff581082)

## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
