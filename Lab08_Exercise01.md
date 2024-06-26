<img width="960" alt="image" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-08/assets/144870609/d512bdc9-088c-4589-80bb-6164e06c7ae0"># Lab 8 Exercise 1

## Class Inheritance

1.สร้าง console application project

```cmd
dotnet new console --name Lab08_Ex01
```

2.เปลี่ยน code ให้เป็นดังต่อไปนี้

```cs
Student student1 = new Student();
student1.Name = "Somchai";
System.Console.WriteLine($"student1 name = {student1.Name}");

var student2 = new Student();
student2.Name = "Sompong";
System.Console.WriteLine($"student2 name = {student2.Name}");

class Person
{
    private string name = string.Empty;
    public string Name
    {
        get { return name; }
        set { name = value; }
    }
}

class Student:Person
{

}
```

3.Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab08_Ex01
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง

4.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3
<img width="960" alt="8 1 1" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-08/assets/144870609/96fb9319-a3d3-40ab-b691-f6a050fa5569">

5.Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab08_Ex01
```

6.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="960" alt="8 1 2" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-08/assets/144870609/9f56851f-9665-45d0-bf30-46d580075bbf">

7.อธิบายสิ่งที่พบในการทดลอง
โปรแกรมจะแสดงผล
student1 name = Somchai
student2 name = Sompong
