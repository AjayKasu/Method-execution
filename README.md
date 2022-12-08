# Method-execution
// how the method execute in different methods.
class Menu
{
	static int y=200;// static varibles declared at inside class
	double x= (double)y;//non-static value stored in main method 
	static void method1() 
		{
			System.out.println("method1");
			System.out.println(y);// accessed only static varibles 
			System.out.println("method1 ends");
		}
		void method2()
		{
			System.out.println("method2");
			System.out.println(y);//varible accessed in instance method
			System.out.println(x);//non-static varible accessed in also method 
			System.out.println("method2 ends");
		}
public static void main (String args[])
	{
		System.out.println("main starts methods:");
		Menu ob= new Menu();//object creation 
		Menu.method1();// method1 call belongs to in static call class
		ob.method2();//method2 call belongs to object non-static 
		System.out.println("mehtod1:"+Menu.y);
		System.out.println("mehtod2:"+ob.x);
		System.out.println("main methods ends:");
	}
}
