# Lab 6 Exercise 3

## Instance vs static members

1. สร้าง console application project

```cmd
dotnet new console --name Lab06_Ex03
```

2. เปลี่ยน code ให้เป็นดังต่อไปนี้

```cs
Person.name = "Enter your name here";
System.Console.WriteLine(Person.GetName());
var student = new Student();
student.name = "Enter student's name";
System.Console.WriteLine(student.GetName());

static class Person
{
    static  public  string? name;
    static  public string GetName()
    {
        return $"Hello from {name}";
    }
}

class Student : Person
{
    
}
```

3. Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab06_Ex03
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง

4. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3 
แก้ไข student.name เป็น Student.name
แก้ไข static public เป็น public startic
6. Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab06_Ex03
```

6. บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="960" alt="6 3 1" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-06/assets/144870609/d70593ea-4457-4fda-a84e-1eae96a9a562">

7. อธิบายสิ่งที่พบในการทดลอง
โปรแกรมจะแสดง Hello Enter your name here,Hello from Enter student's name
