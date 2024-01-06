# 65030258 สิทธา กล้าพานิช 
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

![](./LAB_Images/15.1.png)

#### เป็นการกำหนดตัวแปรและให้ดำเนินการทางคณิตศาสตร์แล้วนำมาแสดงข้อมูลผ่านหน้าจอ 

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
    
```csharp
int a , b , x , y ;

a = 10;

b = 20;

x = 5;

y = 2;

Console.WriteLine("1.a+b={0}", a + b );
Console.WriteLine("2.x-b={0}", x - b );
Console.WriteLine("3.x*b={0}", x * b );
Console.WriteLine("4.y/a={0}", y / a );
Console.WriteLine("5.b%y={0}", b % y );
Console.WriteLine("6.y+10%x={0}", y + 10%x );
Console.WriteLine("7.a/3*5={0}", a / 3*5  );
Console.WriteLine("8.9/2*a={0}", 9 / 2*a  );
Console.WriteLine("9.y%8={0}", y % 8    );
Console.WriteLine("10.100*x+y%2-a={0}", 100 *x+y%2-a );

# Sittha Klaphanich
```
![](./LAB_Images/16.png)


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




👷 คำสั่ง ให้เขียนโปรแกรมคำนวณค่าเพื่อเติมลงในช่องว่างในตาราง
ตารางที่ 1 ระยะทางจากดวงอาทิตย์ถึงดาวเคราะห์ต่างๆ

| ดาวเคราะห์ | ระยะทางจากดวงอาทิตย์ | ระยะทางในหน่วย A.U. | เวลาของแสง (นาที)
|---|---|---|---|
| Mercury | 57,910,000 km | 0.387099 |  3.219454
| Venus | 108,200,000 km | 0.723262 | 6.015282
| Earth | 149,600,000 km | 1.000000 | 8.316877
| Mars | 227,940,000 km | 1.523663 | 12.672119
| Jupiter |  778,330,000 km | 5.202741 | 43.270556
| Uranus | 2,873,550,000 km | 19.208222 | 159.752428
| Neptune | 4,501,000,000 km | 30.086898 | 250.229048
| Pluto | 5,945,900,000 km | 39.745321 | 330.556964

 คลาส Math ในภาษา C# มีคลาสที่เป็นตัวช่วยคำนวณทางคณิตศาสตร์ ที่ช่วยให้เราสามารถคำนวณฟังก์ชันพื้นฐานได้ อย่างรวดเร็ว ไม่ต้องพัฒนาโปรแกรมเพิ่มเติมด้วยเอง นั่นคือคลาส Math ฟังก์ชันทางคณิตศาสตร์ที่ใช้บ่อยๆ สามารถดูรายละเอียดทั้งหมดได้จาก `system.math`
```csharp
double Mercury = 57910000 , Venus = 108200000 , Earth = 149600000 , Mars = 227940000 , Jupiter = 778330000 , Uranus = 2873550000 , Neptune = 4501000000 , Pluto = 5945900000 ;

Console.WriteLine("Mercury A.U.: {0:F6}", Mercury / 149600000);
Console.WriteLine("Venus A.U.:{0:F6}", Venus / 149600000);
Console.WriteLine("Earth A.U.:{0:F6}", Earth / 149600000);
Console.WriteLine("Mars A.U.:{0:F6}", Mars / 149600000);
Console.WriteLine("Jupiter A.U.:{0:F6}", Jupiter / 149600000);
Console.WriteLine("Uranus A.U.:{0:F6}", Uranus / 149600000);
Console.WriteLine("Neptune A.U.:{0:F6}", Neptune / 149600000);
Console.WriteLine("Pluto A.U.:{0:F6}", Pluto / 149600000);
Console.WriteLine("-----------------------------------");
Console.WriteLine("Mercury Time: {0:F6}", Mercury / 299792/60);
Console.WriteLine("Venus Time:{0:F6}", Venus / 299792/60);
Console.WriteLine("Earth Time:{0:F6}", Earth / 299792 / 60);
Console.WriteLine("Mars Time:{0:F6}", Mars / 299792/60);
Console.WriteLine("Jupiter Time:{0:F6}", Jupiter / 299792 / 60);
Console.WriteLine("Uranus Time:{0:F6}", Uranus / 299792 / 60);
Console.WriteLine("Neptune Time:{0:F6}", Neptune / 299792 / 60);
Console.WriteLine("Pluto Time:{0:F6}", Pluto / 299792 / 60);

#Sittha Klaphanich
 ```
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

  
