# Lab 6 Exercise 6

## Member constants

1. สร้าง console application project

```cmd
dotnet new console --name Lab06_Ex06
```

2. เปลี่ยน code ให้เป็นดังต่อไปนี้

```cs
Circle.PrintCircleArea(100);

class Circle
{
    const double PI = 3.14159;
    public static void PrintCircleArea(double radius)
    {
        System.Console.WriteLine($"Radius = {radius}, Area = {PI * radius * radius}");
    }
}
```

3. Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab06_Ex06
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง

4. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3 
<img width="960" alt="6 6 1" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-06/assets/144870609/cec0a6ad-61d5-41f5-9632-54f3b332e9fc">

5. Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab06_Ex06
```

6. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="960" alt="6 6 2" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-06/assets/144870609/3e13f757-3986-4470-993f-f369147bf8b3">

7. อธิบายสิ่งที่พบในการทดลอง
โปรแกรมจะแสดงผล Radius = 100,Area = 31415.8999999998
