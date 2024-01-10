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
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/8ba50c07-4f6f-4f01-9789-9e1fe186d61e)




## 16. หาค่าจากสมการทางคณิตศาสตร์

กำหนด ```a = 10, b = 20, x = 5, y = 2``
👉 ให้เขียนโปรแกรมเพื่อหาผลลัพธ์ของสมการต่อไปนี้

1. `a+b`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/6f6625f2-6655-4967-9265-aadcefa242ea)

2. `x-b`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/e42a28b8-aeb6-4849-8eb3-9ade91cfd10d)

3. `x*b`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/c866cc6c-46be-4f08-af3d-adb4ede9edf8)

4. `y/a`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/c083b107-db53-4cfb-bde0-2bbcce99aaae)

5. `b%y`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/95827129-87d6-4b3f-b176-b196cd6852a3)

6. `y+10%x`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/13cccaae-96f5-425c-a9a0-da225956a790)

7. `a/3*5`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/4b71dfb4-330d-4650-ad4f-4b096bc1a363)

8. `9/2*a`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/db9dd070-1b89-4883-a302-ee74d33d512d)

9. `y%8`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/7abe5c3b-e6ad-46ad-b1f0-29d16e9109a9)

10. `100*x+y%2-a`
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/ab016061-430c-40cf-af87-b7d413332490)

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
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/32047d7b-c065-46e4-868e-8239030baf8d)




👷 คำสั่ง ให้เขียนโปรแกรมคำนวณค่าเพื่อเติมลงในช่องว่างในตาราง
ตารางที่ 1 ระยะทางจากดวงอาทิตย์ถึงดาวเคราะห์ต่างๆ

| ดาวเคราะห์ | ระยะทางจากดวงอาทิตย์ | ระยะทางในหน่วย A.U. | เวลาของแสง (นาที)
|---|---|---|---|
| Mercury | 57,910,000 km |0.000387 A.U. | 0.003219 minutes
| Venus | 108,200,000 km | 0.000723 A.U. | 0.006015 minutes |
| Earth | 149,600,000 km | 0.001000 A.U. | 0.008317 minutes |
| Mars | 227,940,000 km | 0.001524 A.U. | 0.012672 minutes |
| Jupiter |  778,330,000 km | 0.005203 A.U. | 0.043270 minutes |
| Uranus | 2,873,550,000 km | 0.019208 A.U. | 0.159752 minutes |
| Neptune | 4,501,000,000 km | 0.030087 A.U. | 0.250229 minutes |
| Pluto | 5,945,900,000 km | 0.039745 A.U. | 0.330556 minutes |



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
![image](https://github.com/ThanaloekKaisai/03376836-OOP-2566-Lab-01/assets/144195683/cca02624-ba2e-4c25-bfb8-a27969a9ee1f)

  
