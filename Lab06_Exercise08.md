# Lab 6 Exercise 8

## Change constants member value

1. สร้าง console application project

```cmd
dotnet new console --name Lab06_Ex08
```

2. เปลี่ยน code ให้เป็นดังต่อไปนี้

```cs
Circle.PrintCircleArea(100);
class Circle
{
    const double PI = 3.14159;
    public static void PrintCircleArea(double radius)
    {
        PI = 3.14159265359; // change PI to more precision number.
        System.Console.WriteLine($"Radius = {radius}, Area = {PI * radius * radius}");
    }
}
```

3. Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab06_Ex08
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง

4. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3 
<img width="960" alt="6 8 1" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-06/assets/144870609/8332a937-1c8d-4757-9e88-e20bdb3e6fd4">

5. Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab06_Ex08
```

6. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="960" alt="6 8 2" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-06/assets/144870609/9fbcabef-bbff-4160-9daa-e6b4dbb19ebc">

7. อธิบายสิ่งที่พบในการทดลอง
โปรแกรมจะแสดงผล Radius = 100 , Area = 31415.89999998
ไม่สามารถรันได้ เพราะ มีตัวแปร IP ซึ่งไม่สามารถกำหนดค่าได้ เพราะเป็นค่าเฉพาะ
