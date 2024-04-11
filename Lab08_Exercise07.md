# Lab 8 Exercise 7

## Overriding base class member

1. สร้าง console application project

```cmd
dotnet new console --name Lab08_Ex07
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
    public string Hello = "Hello From DerivedClass";
}
```

3.Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab08_Ex07
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง

4.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3
<img width="960" alt="8 7 1" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-08/assets/144870609/d2598abc-3191-41a5-b1e1-74db2a270771">

5.Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab08_Ex07
```

6.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="960" alt="8 7 2" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-08/assets/144870609/816ae81b-463c-4908-bc49-aa3f5fb334b3">

7.อธิบายสิ่งที่พบในการทดลอง
โปรแกรมจะแสดงผล
Hello From DerivedClass
