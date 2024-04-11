# Lab 8 Exercise 9

## Access base member by `base` keyword

1. สร้าง console application project

```cmd
dotnet new console --name Lab08_Ex09
```

2.เปลี่ยน code ให้เป็นดังต่อไปนี้

```cs
DerivedClass dc = new DerivedClass();
dc.PrintBaseHello();

class BaseClass
{
    public string Hello = "Hello From BaseClass";
}
class DerivedClass : BaseClass
{
    new public string Hello = "Hello From DerivedClass";

    public void PrintBaseHello()
    {
        string BaseHello = base.Hello;
        System.Console.WriteLine(BaseHello);
    }
}
```

3.Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab08_Ex09
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง

4.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3
<img width="960" alt="8 9 1" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-08/assets/144870609/06cc1ee2-c664-473c-9322-79f428c46f90">

5.Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab08_Ex09
```

6.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="960" alt="8 9 2" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-08/assets/144870609/51cd5d1b-b97c-4db3-b522-661fc2abd812">

7.อธิบายสิ่งที่พบในการทดลอง
โปรแกรมจะแสดง
Hello From BaseClass
