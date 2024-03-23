# Lab-01  ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)

ข้อมูลชนิดตัวเลขจำนวนเต็ม สามารถนำไปใช้งานได้หลากหลาย เช่น การนับหรือแสดงจำนวน การกำหนดลำดับที่ การจัดลำดับ เป็นต้น ค่าที่ใส่ลงในตัวแปร เป็นได้ทั้งค่าบวก ค่าศูนย์ และค่าลบ (มีตัวแปรบางชนิดที่เก็บเฉพาะค่าบวกเพียงอย่างเดียว) การกำหนดค่าใดๆ ให้กับตัวแปร ทำได้โดยการใช้เครื่องหมาย =
การใช้เครื่องหมายคณิตศาสตร์กับตัวแปรจำนวนเต็ม สามารถใช้ได้ทุกเครื่องหมาย ได้แก่ +, -, *, / และ %

## 15. การใช้เครื่องหมายทางคณิตศาสตร์กับตัวแปรชนิดจำนวนเต็ม

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
int a, b, c, d, e, f;
a = 1;
b = a + 6;
c = b - 3;
d = c * 2;
e = d / 2;
f = e % 2;
Console.WriteLine("a={0}", a);
Console.WriteLine("b={0}", b);
Console.WriteLine("c={0}", c);
Console.WriteLine("d={0}", d);
Console.WriteLine("e={0}", e);
Console.WriteLine("f={0}", f);
```

➢ รันโปรแกรมและบันทึกผล
## ![Screenshot 2024-03-23 230959](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/ba83b3e7-22b1-4e57-a652-8758bc492ff2)




## 16. หาค่าจากสมการทางคณิตศาสตร์

กำหนด ```a = 10, b = 20, x = 5, y = 2``
👉 ให้เขียนโปรแกรมเพื่อหาผลลัพธ์ของสมการต่อไปนี้

1. `a+b`
## ![Screenshot 2024-03-23 231919](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/c62c175b-20a3-4182-b980-1a70f67f9ce9)

2. `x-b`
## ![Screenshot 2024-03-23 231945](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/4c17d4d2-12fb-4e1a-a20e-b6220818ffa8)

3. `x*b`
## ![Screenshot 2024-03-23 232004](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/0b8a1cf1-fff5-4e8f-b9d4-9b5caf8a6d62)

4. `y/a`
## ![Screenshot 2024-03-23 232032](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/37425aa7-028d-4dc4-8fe9-bc056661dfa0)

5. `b%y`
## ![Screenshot 2024-03-23 232103](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/6e073b6f-8760-4822-b196-dadf824d29a2)

6. `y+10%x`
## ![Screenshot 2024-03-23 232141](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/f0870690-65a7-41dc-aa40-a662529bce6d)

7. `a/3*5`
## ![Screenshot 2024-03-23 232222](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/e7386c13-d542-4228-91bd-22bd587deba3)

8. `9/2*a`
## ![Screenshot 2024-03-23 232251](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/0757a18f-ea19-4282-a827-2dd0f9bc67d1)

9. `y%8`
## ![Screenshot 2024-03-23 232314](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/01422d20-e616-4c66-8097-c5e92cd12ee0)

10. `100*x+y%2-a`
## ![Screenshot 2024-03-23 232449](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/3b8699f9-5341-4d4d-9152-ca8c4f62cf95)


## ชนิดข้อมูลเลขทศนิยม (Floating Point and Decimal Types)

ตัวเลขจำนวนทศนิยม มักจะใช้ในการคำนวณทางวิทยาศาสตร์ เนื่องจากค่าในวิทยาศาสตร์ต้องการความละเอียดสูง หรือมีค่าสูงมากกว่าที่เลขจำนวนเต็มจะเก็บได้

### ตัวอย่างการแก้ปัญหาทางวิทยาศาสตร์

ระยะทางจากดาวอาทิตย์ถึงโลกคือ 93,000,000 ไมล์ เรียกว่า 1 A.U. (Astronomical Unit)
ความเร็วในการเดินทางของแสงคือ 186,000 ไมล์ต่อวินาที
ระยะทาง 1 ไมล์ คิดเป็น 1.609344 กิโลเมตร
ให้เขียนโปรแกรมหาระยะทางในการเดินทางของแสง ในหน่วยกิโลเมตรต่อวินาทีและเวลาในการเดินทางของแสงจากดวงอาทิตย์มายังโลก

## 17.  โปรแกรมคำนวณระยะทางและเวลาของแสงจากดวงอาทิตย์ถึงโลก

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
const double lightSpeed = 186000d;   // miles per second
Console.WriteLine("Light speed = {0} Mile Per second", lightSpeed);
const double mileTokm = 1.609344;
Console.WriteLine("Light speed = {0} km Per second", lightSpeed*mileTokm);
const double SunToEarthDistance =  93000000d ;  // miles
Console.WriteLine("SunToEarthDistance = {0} km", SunToEarthDistance * mileTokm);
double SunToEarthTimeOfLight = SunToEarthDistance / lightSpeed;  // miles
Console.WriteLine("SunToEarthTimeOfLight = {0} seconds", SunToEarthTimeOfLight);
Console.WriteLine("SunToEarthTimeOfLight = {0} minutes", SunToEarthTimeOfLight/60d);
```

➢ รันโปรแกรมและบันทึกผล
## ![Screenshot 2024-03-23 232526](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/4cda4477-14a5-4b1d-9ab3-ec71e3bfe1eb)




👷 คำสั่ง ให้เขียนโปรแกรมคำนวณค่าเพื่อเติมลงในช่องว่างในตาราง
ตารางที่ 1 ระยะทางจากดวงอาทิตย์ถึงดาวเคราะห์ต่างๆ

| ดาวเคราะห์ | ระยะทางจากดวงอาทิตย์ | ระยะทางในหน่วย A.U. | เวลาของแสง (นาที)
|---|---|---|---|
| Mercury | 57,910,000 km | 35,983,605 miles | 3.224337365591398 minutes  |
| Venus | 108,200,000 km | 67,232,362 miles| 6.024405197132617 minutes |
| Earth | 149,600,000 km |92,957,130 miles | 8.32949193548387 minutes |
| Mars | 227,940,000 km | 141,635,349 miles |  12.691339516129032 minutes   |
| Jupiter |  778,330,000 km | 483,631,838 miles |  43.336186200716845 minutes |
| Uranus | 2,873,550,000 km | 1,785,541,183 miles | 159.9947296594982 minutes |
| Neptune | 4,501,000,000 km | 2,796,791,726 miles | 250.6085775985663 minutes |
| Pluto | 5,945,900,000 km |  3,694,610,958 miles | 331.05832956989246 minutes |



 คลาส Math ในภาษา C# มีคลาสที่เป็นตัวช่วยคำนวณทางคณิตศาสตร์ ที่ช่วยให้เราสามารถคำนวณฟังก์ชันพื้นฐานได้ อย่างรวดเร็ว ไม่ต้องพัฒนาโปรแกรมเพิ่มเติมด้วยเอง นั่นคือคลาส Math ฟังก์ชันทางคณิตศาสตร์ที่ใช้บ่อยๆ สามารถดูรายละเอียดทั้งหมดได้จาก `system.math`

 
## 20.  โปรแกรมพล็อตรูป sine wave บนหน้าจอ

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
for (float i = 0; i < Math.PI * 2.0F; i += 0.3F)
{
    Console.WriteLine("The sine of {0,10:F} = {1,-10:F6}" + spaces(Math.Sin(i)) + "*", i, Math.Sin(i));
}
string spaces(double val)
{
    string SpaceString = new String(' ', ((int)(val * 10.0)) + 10);
    return SpaceString;
}
```

หมายเหตุ ในการเขียนโปรแกรมภาษา C# .NET6.0 ที่ใช้ template แบบใหม่ เราก็ยังคงสามารถสร้าง function ใช้งานได้ตามปกติ (แต่จะไม่ครอบคลุม feature ทั้งหมดใน OOP )

➢ รันโปรแกรมและบันทึกผล
## ![Screenshot 2024-03-23 232557](https://github.com/ironmanwin1/03376836-OOP-2566-Lab-01/assets/144198724/76d69ff2-7961-4d2b-a097-731305fc0e2a)

  
