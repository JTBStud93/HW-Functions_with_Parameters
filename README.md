# HW-Functions_with_Parameters
Watch read and practice from the module: Functions  Write your understanding of the topic using comments and examples (at least 10 examples) to the instructor and describe them in your own words to the best of your knowledge. Put your work to GIT. Submit the GIT url to canvas. 

1. Based on SoloLearn... In this example, our function is Subtract, whereas our parameters are "int x, int y". So once you print/return x minus y, the result will show a new number.

int Subtract(int x, int y)
{
  return x-y;
}

2. Based on SoloLearn... Should there be multiple parameters, it's important to seperate them (aka arguements) with commas. This will display the value on the console window.

static void Main(string[] args)
{
  Console.Writeline(Sum(4, 5));
}

3. Based on SoloLearn... Another way to do it like the example above, is to make a return value and assign it to a variable.

static void Main(string[] args)
{
  int res = Sum(5, 3);
  Console.Writeline(res);
}

4. Based on SoloLearn... "24" will go through the method as an arguement, and becomes the parameter "x".

public void Print(int x)
{
  Console.Writeline(x);
}
public void Main(string[] args)
{
  Console.Writeline(24);
}

OUTPUT
24

5. Based on SoloLearn... Even in the same method, various arguements can go through, as long as they're a certain datatype.

public void Func(int x)
{
  Console.Writeline(x*3);
}
public void Main(String[] args)
{
  Func(3);
  Func(10);
  Func(30);
}

OUTPUT
9
30
90

6. Based on SoloLearn... Output parameters can move information outside of the method, and not take other info in.

public void GetValues(out int x, out int y)
{
  x = 7;
  y = 11;
}
public void Main(string[] args)
{
  int a, b;
  GetValues(out a, out b);
}

OUTPUT
a = 7
b = 11

7. Page 40-41 in the book... In this example, we see that the "Main" function has Foo assigned to x, which is assigned to 8. In the Foo function above, Foo is now assigned to "p", as well as increasing "8" by 1. So this prints as 8 & 9.

public class FuncParameters : MonoBehaviour {

  public void Foo (int p)
  {
    p = p + 1;
    print(p);
  }
  public void Main()
  {
    int x = 8;
    Foo (x);
    print(x);
  }

}

OUTPUT
//9
//8

8. Page 42 in the book... Similar to #7 above, since Foo/x/8 is used by a "ref" keyword (reference), it duplicates the argument in the first parameter below. This lets the method to work on the variable.

public class FuncParameters : MonoBehaviour {

  public void Foo (ref int p)
  {
    p = p + 1;
    print(p);
  }
  public void Main()
  {
    int x = 8;
    Foo (ref x);
    print(x);
  }
}

OUTPUT
//9
//9

9. Based on SoloLearn... Fact is also known as (x!). Which would be something like: 4! = 4*3*2*1 = 24.

public void Main(string[] args)
{
  print(Fact(10));
}

OUTPUT
3,628,800

10. Based on SoloLearn... The "(By) Value" duplicates the value of the argument, and gets placed in the parameter (int z). This allows us to alter the parameter inside the method without impacting the arguement.

public void Sqr(int z)
{
  z = z * z;
}
public void Main()
{
int b = 9;
Sqr(b);

Console.Writeline(b);
}
