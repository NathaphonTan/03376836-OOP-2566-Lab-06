# Lab 6 Exercise 1

## การใช้งาน Modifier

1. สร้าง console application project

```cmd
dotnet new console --name Lab06_Ex01
```

2. เปลี่ยน code ให้เป็นดังต่อไปนี้

```cs
Person.name = "Enter your name here";
System.Console.WriteLine(Person.GetName());

static class Person
{
    public static string? name;
    public static string GetName()
    {
        return $"Hello from {name}";
    }
}
```

3. Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab06_Ex01
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง

4. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3

5. Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab06_Ex01
```

6. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="960" alt="6 1 1" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-06/assets/144870609/ddee13a0-988f-4f26-bcf9-72b7dfb913da">

7. อธิบายสิ่งที่พบในการทดลอง
โปรแกรมจะแสดงผล Hello foem Enter your name here สร้าง Person ที่มี Field name Method Getname() เพื่อคืนค่า Hello from พร้อมกับค่า name ที่กำหนด 
