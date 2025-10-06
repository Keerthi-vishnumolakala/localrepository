Employee employee=new Employee(); 

&nbsp;	System.out.println("Enter employee details:");

&nbsp;	System.out.println("Enter employee Number:");

&nbsp;	int emp=sc.nextInt();

&nbsp;	sc.nextLine();

&nbsp;	System.out.println("Enter employee name:");

&nbsp;	String ename=sc.nextLine();

&nbsp;	System.out.println("Enter employee basic salary:");

&nbsp;	double bp=sc.nextDouble();

hiiii

### **NO Argument constructor**

**------------------------------------------------------------------**

**No argument is same as default constructor but default constructor is handled by the machine only but we give data in no argument**

int emp;

String ename;

double bp;



public Employee(){   //to write a constructor,we need instance variables

&nbsp;	emp=0;

&nbsp;	ename=null;

&nbsp;	bp=0;  //even bp is double int to double conversion can happen so no problem

&nbsp;	}



### **Parameterized constructor**

**---------------------------------------------------------------------**



**Employee employee=new Employee(emp,ename,bp); //during creating an object give parameters only**



public Employee(int emp,String ename,double bp){

&nbsp;		emp=emp;

&nbsp;		ename=ename;

&nbsp;		bp=bp;

&nbsp;	}

the machine dont understand why you are using local variables and assigning so we use "this" keyword



this is a reference that points to the current variable



public Employee(int emp,String ename,double bp){

&nbsp;		this.emp=emp;

&nbsp;		this.ename=ename;//the colour of ename,emp,bp changed telling that those are instance variables.

&nbsp;		this.bp=bp;



}



Employee emp1=new Employee(101,"Vijay", 10000);

System.out.println("Emp no:"+emp1.emp+"\\nEmployee Name:"+emp1.ename+"\\nEmployee Salary:"+emp1.calc\_salary());

//employee.emp refers to the instance variables in constructor instead of using local variables we use instance   variables



System.out.println();



Employee emp2=new Employee(102,"Vishali", 20000);

System.out.println("Emp no:"+emp2.emp+"\\nEmployee Name:"+emp2.ename+"\\nEmployee Salary:"+emp2.calc\_salary());

&nbsp;		sc.close();

### **Copy constructor**

**--------------------------------------------**

**instead of creating a new object it referes to the same object**



**Employee emp3=emp2;**



**it copies the data which is in emp2 and gives in emp3.**



### **Access Modifiers**

**--------------------------------------------**



**public**

**protected**

**private**

**default**



for variables dont use public and default because it can be accessed by everyone

use private and protected



**do not write instance variables in public use private**



**constructors are always public**



**we cant access variables if they are private so we can access them by using getters and setters**



**//getter**

**public String getName(){**

**return name;**

**}**



**//setter**

**public void setName(String name){**

**this.name=name;**

**}**

**\*\*\*\*\*\*\*\*\***

### **String**

**-----------------------------**

**string**

**string builder**

**string buffer**



**StringBuilder**(we use only string builder)



Not thread-safe (no synchronization).

Faster than StringBuffer in single-threaded environments.



String Buffer



Thread-safe(Synchronized)

slower-->works with multiple things





