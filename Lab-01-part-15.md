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

![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/b1763cc0-517a-45ac-8d25-9688eb1e6d27)



## 16. หาค่าจากสมการทางคณิตศาสตร์

กำหนด ```a = 10, b = 20, x = 5, y = 2``
👉 ให้เขียนโปรแกรมเพื่อหาผลลัพธ์ของสมการต่อไปนี้

1. `a+b`
2. `x-b`
3. `x*b`
4. `y/a`
5. `b%y`
6. `y+10%x`
7. `a/3*5`
8. `9/2*a`
9. `y%8`
10. `100*x+y%2-a`
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/3ec824e4-a666-4005-8e89-37212ba02463)

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
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/a340c644-1ecb-4808-8121-0c302893dba8)




👷 คำสั่ง ให้เขียนโปรแกรมคำนวณค่าเพื่อเติมลงในช่องว่างในตาราง
ตารางที่ 1 ระยะทางจากดวงอาทิตย์ถึงดาวเคราะห์ต่างๆ

| ดาวเคราะห์ | ระยะทางจากดวงอาทิตย์ | ระยะทางในหน่วย A.U. | เวลาของแสง (นาที)
|---|---|---|---|
| Mercury | 57,910,000 km | 0.000387 A.U.| 0.003219 minutes |
| Venus | 108,200,000 km | 0.000723 A.U. | 0.006015 minutes |
| Earth | 149,600,000 km | 0.001000 A.U.| 0.008317 minutes |
| Mars | 227,940,000 km | 0.001524 A.U. | 0.012672 minutes |
| Jupiter |  778,330,000 km | 0.005203 A.U. | 0.043270 minutes |
| Uranus | 2,873,550,000 km | 0.019208 A.U.|  0.159752 minutes |
| Neptune | 4,501,000,000 km | 0.030087 A.U.| 0.250229 minutes |
| Pluto | 5,945,900,000 km | 0.039745 A.U. | 0.330556 minutes |
##
👉
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/fbce5bd6-69ba-44bc-afac-fd0dc7347ff4)
```
using System;

class Program
{
    static void Main()
    {
        // ค่าคงที่
        const double SpeedOfLight = 299792458.0; // ความเร็วแสงในวิกฤตต่อวินาที (เมตร)

        // ระยะทางจากดวงอาทิตย์ถึงดาวเคราะห์ (เมตร)
        double distanceToSun_Mercury = 57910000;
        double distanceToSun_Venus = 108200000;
        double distanceToSun_Earth = 149600000;
        double distanceToSun_Mars = 227940000;
        double distanceToSun_Jupiter = 778330000;
        double distanceToSun_Uranus = 2873550000;
        double distanceToSun_Neptune = 4501000000;
        double distanceToSun_Pluto = 5945900000;

        // คำนวณระยะทางในหน่วย A.U.
        double auConversion = 1.496e11; // 1 A.U. = 149.6 ล้าน กิโลเมตร
        double distanceAU_Mercury = distanceToSun_Mercury / auConversion;
        double distanceAU_Venus = distanceToSun_Venus / auConversion;
        double distanceAU_Earth = distanceToSun_Earth / auConversion;
        double distanceAU_Mars = distanceToSun_Mars / auConversion;
        double distanceAU_Jupiter = distanceToSun_Jupiter / auConversion;
        double distanceAU_Uranus = distanceToSun_Uranus / auConversion;
        double distanceAU_Neptune = distanceToSun_Neptune / auConversion;
        double distanceAU_Pluto = distanceToSun_Pluto / auConversion;

        // คำนวณเวลาของแสง (นาที)
        double timeLightMinutes_Mercury = distanceToSun_Mercury / SpeedOfLight / 60;
        double timeLightMinutes_Venus = distanceToSun_Venus / SpeedOfLight / 60;
        double timeLightMinutes_Earth = distanceToSun_Earth / SpeedOfLight / 60;
        double timeLightMinutes_Mars = distanceToSun_Mars / SpeedOfLight / 60;
        double timeLightMinutes_Jupiter = distanceToSun_Jupiter / SpeedOfLight / 60;
        double timeLightMinutes_Uranus = distanceToSun_Uranus / SpeedOfLight / 60;
        double timeLightMinutes_Neptune = distanceToSun_Neptune / SpeedOfLight / 60;
        double timeLightMinutes_Pluto = distanceToSun_Pluto / SpeedOfLight / 60;

        // แสดงผลลัพธ์
        Console.WriteLine("| Mercury   | {0} km | {1:F6} A.U. | {2:F6} minutes |", distanceToSun_Mercury, distanceAU_Mercury, timeLightMinutes_Mercury);
        Console.WriteLine("| Venus     | {0} km | {1:F6} A.U. | {2:F6} minutes |", distanceToSun_Venus, distanceAU_Venus, timeLightMinutes_Venus);
        Console.WriteLine("| Earth     | {0} km | {1:F6} A.U. | {2:F6} minutes |", distanceToSun_Earth, distanceAU_Earth, timeLightMinutes_Earth);
        Console.WriteLine("| Mars      | {0} km | {1:F6} A.U. | {2:F6} minutes |", distanceToSun_Mars, distanceAU_Mars, timeLightMinutes_Mars);
        Console.WriteLine("| Jupiter   | {0} km | {1:F6} A.U. | {2:F6} minutes |", distanceToSun_Jupiter, distanceAU_Jupiter, timeLightMinutes_Jupiter);
        Console.WriteLine("| Uranus    | {0} km | {1:F6} A.U. | {2:F6} minutes |", distanceToSun_Uranus, distanceAU_Uranus, timeLightMinutes_Uranus);
        Console.WriteLine("| Neptune   | {0} km | {1:F6} A.U. | {2:F6} minutes |", distanceToSun_Neptune, distanceAU_Neptune, timeLightMinutes_Neptune);
        Console.WriteLine("| Pluto     | {0} km | {1:F6} A.U. | {2:F6} minutes |", distanceToSun_Pluto, distanceAU_Pluto, timeLightMinutes_Pluto);
    }
}

```
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/2380fe12-4215-4877-9410-1a7c851f98ee)



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
![image](https://github.com/Phetteepop/03376836-OOP-2566-Lab-01/assets/144197367/a5406091-d44c-463c-a0e9-4aafffc16454)

  
