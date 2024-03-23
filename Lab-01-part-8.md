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
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/fe6c1d9d-b2fc-419b-b5b7-11dcade51377)
จากการทดลอง Console.WriteLine("{0:Fn}", i); แสดงค่าตัวแปรi ในรูปแบบทศนิยม โดยใช้รูปแบบ F คือ ระบุจำนวนทศนิยมที่ต้องการแสดงหลังจุดทศนิยม F1-F5 คือ แสดงเลขทศนิยมของตัวแปร i ที่มี1-4 ตำแหน่งทศนิยม (ภาพรวมแต่ละบรรทัด) 
## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/75ec8416-b711-4d63-aa5d-b928b56bd7d4)

``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/43c7e828-0d1c-4025-ae1e-8c3ac0fbed91)

``` csharp
3. Console.WriteLine("Hello " + "World");
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/1033e480-5869-4eba-8e9a-8fa6d758e730)

``` csharp
4. Console.WriteLine("Here comes a slash \\");
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/32110d48-3a84-4e3e-8055-5a1be32dcf81)

``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/30fdbd90-b93e-417d-bf54-599ea3334749)

``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/d70d98a1-825f-4575-95e6-a12251494f8d)

``` csharp
7. Console.WriteLine("The value: {0}.", 500);
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/3cad84d7-a35c-429b-ad6b-642c363dfbe9)

``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/1715c95d-2a39-4690-9778-4e9ca353bc94)

``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/edc829a2-9d80-44c4-8d6e-7edd31e87633)

``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/c44042c7-4dad-44c7-bfa8-8e5e38aa456d)

``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/be7df10b-cec1-43cc-9e2d-88801018a5f1)

``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/310c6547-5940-4183-839b-bdb9ed99ce24)

``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/91de6435-85d3-473b-a264-9001cc6f37a3)

``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/8723b475-134a-4097-9878-b28433ad3efa)

``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
```
![image](https://github.com/65030121natthamon/03376836-OOP-2566-Lab-01/assets/144195611/c323b273-c86e-48a0-86b0-0de15be1da5d)



## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
