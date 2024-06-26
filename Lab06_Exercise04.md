# Lab 6 Exercise 4

## Instance vs static members

1. สร้าง console application project

```cmd
dotnet new console --name Lab06_Ex04
```

2. เปลี่ยน code ให้เป็นดังต่อไปนี้

```cs
var a1 = new AAA();
var a2 = new AAA();
a1.b1 = 10;
AAA.b2 = 20;
a2.b1 = 30;
a2.b2 = 40;

System.Console.WriteLine($"a1.b1 = {a1.b1}");
System.Console.WriteLine($"AAA.b2 = {AAA.b2}");
System.Console.WriteLine($"a2.b1 = {a2.b1}");
System.Console.WriteLine($"a2.b2 = {a2.b2}");

class AAA 
{
    public int b1;
    public static int b2;

}
```

3. Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab06_Ex04
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง

4. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3
   แก้ไขโดยให้ a2.b2. เป็น AA.b2
5. Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab06_Ex04
```

6. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="960" alt="6 4 1" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-06/assets/144870609/c6f3c2d9-b689-4760-a936-9feddb326cf6">

7. อธิบายสิ่งที่พบในการทดลอง
โปรแกรมจะแสดงผล a1.b1 = 10 AAA.b2 = 40 a2.b1= 30 a2.b2 = 40
