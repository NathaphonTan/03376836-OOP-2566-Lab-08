# Lab 8 Exercise 10

## Using a references to a base class

1. สร้าง console application project

```cmd
dotnet new console --name Lab08_Ex10
```

2.เปลี่ยน code ให้เป็นดังต่อไปนี้

```cs
DerivedClass DC = new DerivedClass();
System.Console.WriteLine($"DC.Field1 = {DC.Field1}");
BaseClass BC = (BaseClass)DC;
System.Console.WriteLine($"BC.Field1 = {BC.Field1}");

class BaseClass
{
    public string Field1 = "Field1 of BaseClass"; 
}
class DerivedClass:BaseClass
{
    new public string Field1 = "Field1 of DerivedClass"; 
}
```

3.Build project โดยการใช้คำสั่ง

```cmd
dotnet build  Lab08_Ex10
```

ถ้ามีที่ผิดพลาดในโปรแกรม ให้แก้ไขให้ถูกต้อง

4.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 3
<img width="960" alt="8 10 1" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-08/assets/144870609/e98db813-0d1a-4502-9059-4d836b978092">

5.Run project โดยการใช้คำสั่ง

```cmd
dotnet run --project Lab08_Ex10
```

6.บันทึกผลที่ได้จากการรันคำสั่งในข้อ 5
<img width="960" alt="8 10 2" src="https://github.com/NathaphonTan/03376836-OOP-2566-Lab-08/assets/144870609/ec3d0b89-e046-482b-978b-a625f65442d6">

7.อธิบายสิ่งที่พบในการทดลอง
โปรแกรมจะแสดงผล
DC.Field1 = Field1 of DerivedClass
BC.Field1 = Field1 of BaseClass
