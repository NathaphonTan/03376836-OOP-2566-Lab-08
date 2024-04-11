# Lab 8 Exercise 8

## Masking base class member with `new` keyword

1. สร้าง console application project

```cmd
dotnet new console --name Lab08_Ex08
```

2.เปลี่ยน code ให้เป็นดังต่อไปนี้

```cs
DerivedClass dc = new DerivedClass();
System.Console.WriteLine(dc.Hello);

class BaseClass
{
    public string Hello = "Hello From BaseClass";
}
class DerivedClass : BaseClass
{
    new public string Hello = "Hello From DerivedClass";
}
```

3.Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab08_Ex08
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง

4.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3
<img width="960" alt="8 8 1" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-08/assets/144870609/73324a5a-40f2-494e-9494-ae7995cdc798">

5.Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab08_Ex08
```

6.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="960" alt="8 8 2" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-08/assets/144870609/cb93eabf-0142-4f4e-9fa1-52e1132a4192">

7.อธิบายสิ่งที่พบในการทดลอง
โปรแกรมจะแสดงผล
Hello From DerivedClass
