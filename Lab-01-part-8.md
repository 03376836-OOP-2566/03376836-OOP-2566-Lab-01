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
<img width="722" alt="Screenshot 2024-03-23 200944" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/f3f9cb20-899c-48f8-9cc8-21a01a041e3f">

## ❔ แบบฝึกหัด จงรันโปรแกรมและบันทึกภาพ output ของบรรทัดคำสั่งต่อไปนี้

``` csharp
1. string name = "Hello";
    Console.WriteLine(String.Format("{0} there. I said {0}! {0}???", name));
```

<img width="721" alt="Screenshot 2024-03-23 200958" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/62ec8937-a685-4fb6-b145-961b2af553cf">

``` csharp

2. Console.WriteLine("{2:d} {0:d} {1:d}", 1, 2, 3);
```
<img width="720" alt="Screenshot 2024-03-23 201022" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/ed042c23-bd97-4328-b65d-89739b0dba51">

``` csharp

3. Console.WriteLine("Hello " + "World");
```
<img width="717" alt="Screenshot 2024-03-23 201033" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/74771406-ff4e-48ec-9c18-87d85dc151ca">

``` csharp

4. Console.WriteLine("Here comes a slash \\");
```
<img width="721" alt="Screenshot 2024-03-23 201045" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/f7ab888a-dc6a-4de0-a832-65121b5f469f">

``` csharp

5. Console.WriteLine("|{0, 10}|", 999);
```
<img width="716" alt="Screenshot 2024-03-23 201055" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/59ea7d9c-415d-4089-b08e-302a7d7eca2e">

``` csharp

6. Console.WriteLine("|{0,-10}|", 000);
```
<img width="715" alt="Screenshot 2024-03-23 201107" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/7c0123e8-d7fa-41b4-b3ec-71671798f9c5">

``` csharp

7. Console.WriteLine("The value: {0}.", 500);
```
<img width="717" alt="Screenshot 2024-03-23 201118" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/cd780680-a4c6-458d-b066-70007a94f22e">

``` csharp

8. Console.WriteLine("The value: {0:C}.", 500);
```
<img width="715" alt="Screenshot 2024-03-23 201126" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/8067f611-161e-4a54-99ae-a27206c2883f">

``` csharp

9. Console.WriteLine("{0,-10:F4}", 12.3456789);
```
<img width="721" alt="Screenshot 2024-03-23 201139" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/7341d65f-452c-49af-b545-036beb205f2b">

``` csharp

10. Console.WriteLine("{0,-10:C}", 12.3456789);
```
<img width="722" alt="Screenshot 2024-03-23 201148" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/40cccaff-0e41-4e63-bf9f-0868616faf36">

``` csharp

11. Console.WriteLine("{0,-10:E3}", 12.3456789);
```
<img width="722" alt="Screenshot 2024-03-23 201155" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/59c5b53f-5dd6-45c2-a1fe-875748183ed8">

``` csharp

12. Console.WriteLine("{0,-10:x}", 65535);  // (x = lower case)
```
<img width="720" alt="Screenshot 2024-03-23 201206" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/5abb1c57-b9d1-4ca0-ae50-845eee8dee76">

``` csharp

13. Console.WriteLine("{0,-10:X}", 65535);  // (X = upper case)
```
<img width="720" alt="Screenshot 2024-03-23 201214" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/1412f212-5852-4d67-b218-cce5957592b4">

``` csharp

14. int i;
    Console.WriteLine("Value\tSquared\tCubed");
    for(i = 1; i < 10; i++)
        Console.WriteLine("{0}\t{1}\t{2}", i, i*i, i*i*i);
```
<img width="719" alt="Screenshot 2024-03-23 201225" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/5fc1d5b0-7057-40f8-9c93-adb51e484ef6">

``` csharp

15. Console.WriteLine("{0:#.###}.", 1234.56789);
```
<img width="721" alt="Screenshot 2024-03-23 201234" src="https://github.com/SuphawadiP/03376836-OOP-2566-Lab-01/assets/144196049/40f96a32-ced2-4dd4-b9ef-ea23a572beed">


## [การใช้งานคำสั่ง Console.Read() และ Console.ReadLine()](./Lab-01-part-9-12.md)
