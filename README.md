# HW-Functions_with_Parameters
Watch read and practice from the module: Functions  Write your understanding of the topic using comments and examples (at least 10 examples) to the instructor and describe them in your own words to the best of your knowledge. Put your work to GIT. Submit the GIT url to canvas. 

1. 

int Subtract(int x, int y)
{
  return x-y;
}

2. 

static void Main(string[] args)
{
  Console.Writeline(Sum(4, 5));
}

3. 

static void Main(string[] args)
{
  int res = Sum(5, 3);
  Console.Writeline(res);
}

4. 

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

5. SoloLearn

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

6. SoloLearn

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

7. page 40-41

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

8. page 42

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

9. SoloLearn (x!)

public void Main(string[] args)
{
  print(Fact(10));
}

OUTPUT
3,628,800

10.

class Main()
{

  int key = Treasure;

  switch (Treasure == True)
  {
    case "Treasure":
      print ("You're rich now!);
      break;
    case "Empty":
      print ("Welp, you just wasted a key...);
      break;
    case "Mimic":
      print ("You got eaten.");
      break;
    default:
      print ("I'll save the key for later.");
      break;
  }
}

OUTPUT:
"You're rich now!"
