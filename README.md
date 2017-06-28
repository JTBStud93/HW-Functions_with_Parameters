# HW-Functions_with_Parameters
Watch read and practice from the module: Functions  Write your understanding of the topic using comments and examples (at least 10 examples) to the instructor and describe them in your own words to the best of your knowledge. Put your work to GIT. Submit the GIT url to canvas. 

1. Unity Tutorial

public class FuncParameters : MonoBehaviour {

  int myInt = 3;

  void Start(){
    myInt = MultiplyByThree(myInt);
    print(myInt);
  }

  int MultiplyByThree(int number){
    int ret;

    ret = number * 3;

    return ret;
  }

}

OUTPUT
//9

2. page 40-41

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

3. page 42

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

4. SoloLearn

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

5. SoloLearn (x!)

public void Main(string[] args)
{
  print(Fact(10));
}

OUTPUT
3,628,800

6.



7.



8.



9.



10.

