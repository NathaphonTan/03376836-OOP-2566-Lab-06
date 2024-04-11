# Lab 6 Exercise 2

## การใช้งาน Modifier


1. สร้าง console application project

```
dotnet new console --name Lab06_Ex02
```
2. เปลี่ยน code ให้เป็นดังต่อไปนี้

```cs
Person.name = "Enter your name here";
System.Console.WriteLine(Person.GetName());

static class Person
{
    static public  string? name;
    static public  string GetName()
    {
        return $"Hello from {name}";
    }
}
```

3. Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab06_Ex02
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง


4. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3

5. Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab06_Ex02
```

6. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="960" alt="6 2 1" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-06/assets/144870609/4b989648-f8ee-4110-b1f4-9c12bcc1a30e">

7. อธิบายสิ่งที่พบในการทดลอง
การสลับ static และ public ไม่เกิดผลกระทบใดๆ ในกรณีนี้ เนื่องจาก static ถูกใช้กับ class ทำให้ตัวแปรและ method ที่อยู่ใน Class นั้นสามารถเข้าถึงได้โดยไม่ต้องสร้าง instance ของ class นั้นๆ ดังนั้นไม่ส่าจะประกาศ static ก่อนหรือหลัง public ก็ไม่มีผลต่อการทำงานของโปรแกรม
