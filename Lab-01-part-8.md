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
<img width="857" alt="Screenshot 2024-03-23 210359" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/b050ba7d-93ca-4380-ad20-6803624ec965">


## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
<img width="863" alt="Screenshot 2024-03-23 211600" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/fff1d338-95e7-4042-a7ef-1a26440b3b40">

```
``` csharp
2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
<img width="853" alt="Screenshot 2024-03-23 211636" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/9901a016-104e-4f40-affe-046410605879">

```
``` csharp
3. Console.WriteLine("Hello " + "World");
<img width="853" alt="Screenshot 2024-03-23 211657" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/92f45370-f5b4-47b7-8f1b-9e6eac259223">

```
``` csharp
4. Console.WriteLine("Here comes a slash \\");
<img width="856" alt="Screenshot 2024-03-23 211740" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/6a53c4e5-1900-4fec-a660-70e4dd402243">

```
``` csharp
5. Console.WriteLine("|{0, 10}|", 999);
<img width="865" alt="Screenshot 2024-03-23 211803" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/d2340b1e-4ad7-4a57-8230-4f2450c7ac97">

```
``` csharp
6. Console.WriteLine("|{0,-10}|", 000);
<img width="860" alt="Screenshot 2024-03-23 211838" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/d15259a9-5e1d-438c-b6ad-b0208030830a">

```
``` csharp
7. Console.WriteLine("The value: {0}.", 500);
<img width="862" alt="Screenshot 2024-03-23 214739" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/edbb0853-25ac-447a-9e2b-4cc3f9a7b84c">

```
``` csharp
8. Console.WriteLine("The value: {0:C}.", 500);
<img width="858" alt="Screenshot 2024-03-23 214804" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/38f94066-8e64-4551-904b-9a52a15b0e52">

```
``` csharp
9. Console.WriteLine("{0,-10:F4}", 12.3456789);
<img width="860" alt="Screenshot 2024-03-23 214843" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/f434e05c-5260-4908-aedf-f8e2c945b09d">

```
``` csharp
10. Console.WriteLine("{0,-10:C}", 12.3456789);
<img width="861" alt="Screenshot 2024-03-23 214937" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/e60755c4-288a-45ad-8e12-ab6ca3787c4e">

```
``` csharp
11. Console.WriteLine("{0,-10:E3}", 12.3456789);
<img width="859" alt="Screenshot 2024-03-23 215259" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/ee21a67a-4798-4fcd-bae9-d96a04a356fb">

```
``` csharp
12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
<img width="862" alt="Screenshot 2024-03-23 215329" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/174a4a39-0092-44ae-8fa7-b0121068b3d4">

```
``` csharp
13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
<img width="856" alt="Screenshot 2024-03-23 215418" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/8948a481-d56d-4d5a-bcd5-2b424a8789a2">

```
``` csharp
14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
<img width="862" alt="Screenshot 2024-03-23 215612" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/b3d0f99a-1697-4088-b8f2-1cb0233ef95e">

```
``` csharp
15. Console.WriteLine("{0:#.###}.", 1234.56789);
<img width="854" alt="Screenshot 2024-03-23 215638" src="https://github.com/anndyyzzz/03376836-OOP-2566-Lab-01/assets/144866059/c7023ffc-3725-4fd1-abcb-2ed9ea8fadf8">

```


## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
