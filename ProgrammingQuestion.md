


### Swap Two Numbers:

###### Swap Two Numbers with out using Thrid Number:

```

// Online Java Compiler
// Use this editor to write, compile and run your Java code online

class SwapTwoNumber {
    public static void main(String[] args) {
        int a =10, b = 20;
        
        a=a+b;
        b=a-b;
        a=a-b;
        
        
        System.out.println(a+" ");
        System.out.println(b);
    }
}

```



### Swap two numbers:

int a =10,b=20;

a=a+b;
a=a-b;
b=a-b;


### Reverse numbers:

```
Scanner sc = new Scanner(System.in);

int num= sc.nextInt();

options 1:

StringBuffer sb = new StringBuffer(String.valueOf(num));
sb.reverse();
 
System.out.println(sb);

options 2:

sb.append(num);
sb.reverse();
```
### Revese String:

options 1:
```
    public static void main(String []args) {
        String sc ="sandy";
        String rev = "";
        char a[]= sc.toCharArray(); //sandy
        for(int i=sc.length()-1; i>=0; i--) {
            rev = rev + a[i];
        }
        System.out.println(rev);
    }

options 2:

   public static void main(String []args) {
            String sc = "tteess";
        StringBuffer sb = new StringBuffer(sc);
        System.out.println(sb.reverse());
    }
```
### Palindrome:

```
public static void main(String []args) {
        String org = "ava";
        String rev = "";
        int n= org.length();
        char c [] = org.toCharArray();
        for(int i=n-1; i>=0; i--)
            rev = rev + c[i];
        if(org.equals(rev))
            System.out.println("palindrome");
        else
            System.out.println("not palindrome");

    }


```
### String equal or not:

```
public static void main(String []args) {
        String org = "ava";
        String rev = "";
        int n= org.length();
        char c [] = org.toCharArray();
        for(int i=n-1; i>=0; i--)
            rev = rev + c[i];
        if(org.equals(rev))
            System.out.println("palindrome");
        else
            System.out.println("not palindrome");
}


#### Count Number Of Digits in A Number:


/* Online Java Compiler and Editor */
public class HelloWorld {
    public static void main(String []args) {
        int num = 12345;
        int count = 0;
        while(num>0) {
            num = num / 10;
            count++;
        }
        System.out.println("Count " +count);
    }
}
```
#### Even numbers and odd numbers:
```
/* Online Java Compiler and Editor */
public class HelloWorld {
    public static void main(String []args) {
        int num = 1234;
        if(num%2==0) {
            System.out.println("even " +num);
        }
        else {
            System.out.println("odd " +num);
        }
    }
}
```
#### count sum of digits:
```
/* Online Java Compiler and Editor */
public class HelloWorld {
    public static void main(String []args) {
        int num = 12345;
        int sum= 0;
        while(num>0) {
            sum = sum+num%10;
            num = num / 10;
        }
        System.out.println(sum);
    }
}
```

#### highest of three numbers:

```
/* Online Java Compiler and Editor */
public class HelloWorld {
    public static void main(String []args) {
        int a =200 ,b=1000, c = 30;
        if(a > b && a > c )
            System.out.println(" A is Bigger " + a );
        else if(b>a && b>c )
            System.out.println(" B is Bigger " + b );
        else
            System.out.println(" C is Bigger " + c );
    }
}
```

#### Fibonacci Series:
```
hint:

0 1 1 2 3 5 7 12 21 35

0
/* Online Java Compiler and Editor */
public class HelloWorld {
    public static void main(String []args) {
        int  n1 = 0, n2 =1, sum= 0;
        System.out.print(n1+" "+n2);
        for ( int i=2; i<10; i++) {
            sum = n1+n2;
            System.out.print(" "+sum);
            n1=n2;
            n2=sum;
        }
    }
}
```

#### Swap two number:
```
 a =  a+ b;
 a = a - b;
 b = a - b;

/* Online Java Compiler and Editor */
public class HelloWorld {
    public static void main(String []args) {
        int a =10, b=20;
        a =  a+ b;
        b = a - b;
        a = a - b;
        System.out.println("a "+a);
        System.out.print("b "+b);
    }
}
```
### Two Equal array:
```
import java.util.*;
public class HelloWorld {
    public static void main(String []args) {
        int a1[] = {1,2,3,4,5};
        int b1[] = {1,2,3,4};
        boolean yes = Arrays.equals(a1,b1);
        if(yes)
            System.out.println("Yes");
        else
            System.out.println("No");
    }
}
```
Options 2:
```
/* Online Java Compiler and Editor */

import java.util.*;
public class HelloWorld {
    public static void main(String []args) {
        int a1[] = {1,2,3,6};
        int b1[] = {1,2,3,4};
        boolean status = false;
        if(a1.length ==b1.length)
            for(int i=0; i<a1.length; i++) {
                if(a1[i]==b1[i])
                    status = true;
                else
                    status = false;
                }

        if(status) {
            System.out.println("Yes");
        } else {
            System.out.println("No");
        }
    }

}
```
#### Max number in array:
```
/* Online Java Compiler and Editor */

import java.util.*;
public class HelloWorld {
    public static void main(String []args) {
        int a[] = {1,2,23,6};
        int max = 0;
        for(int i=0; i<a.length; i++) {
            if(a[i]>max)
                max = a[i];
        }
        System.out.println(max);
    }
}
```
#### Min Number in array:
```
/* Online Java Compiler and Editor */

import java.util.*;
public class HelloWorld {
    public static void main(String []args) {
        int a[] = {11,222,23,66};
        int min =a[0];
        for(int i=0; i<a.length; i++) {
            if(a[i]<min)
                min = a[i];
        }
        System.out.println(min);
    }
}
```

#### Duplicate in string:

```

/* Online Java Compiler and Editor */

import java.util.*;
public class HelloWorld {
    public static void main(String []args) {
        String name [] = { "sandy","mandy","pandy","sandy"};
        boolean checkstatus = false;
        for(int i=0; i<name.length; i++)
            for(int j=i+1; j<name.length; j++)
                if(name[i]==name[j])
                    checkstatus= true;

        if(checkstatus)
            System.out.println("Duplicate found");
        else
            System.out.println("No Duplicate");
    }
}
```

### Index of element:
```
/* Online Java Compiler and Editor */

import java.util.*;
public class HelloWorld {
    public static void main(String []args) {
        int a[]= {10,20,35,40,50};
        int search = 35;
        int count = 0;
        for(int i=0; i<a.length; i++)
            if(a[i]==search) {
                System.out.println("Element found "+ i);
            }
    }
}


```
#### replase Special Character:


```
/* Online Java Compiler and Editor */

import java.util.*;
public class HelloWorld {
public static void main(String []args) {
String s ="asda1!#$@#$#$@#$@#@#$@# dsadasd";
s =a.replaceAll(("[^a-bA-B0-9]"),"");
System.out.println(s);
}
}

```

#### Sort in Arrays:

```
/* Online Java Compiler and Editor */
import java.util.*;
public class HelloWorld {
    public static void main(String []args) 
    {
        int a[]={20,30,10,50,99};
        System.out.println("Before sort" +Arrays.toString(a));
        Arrays.sort(a);
        System.out.println("After sort" +Arrays.toString(a));
    }
}


output:

Before sort[20, 30, 10, 50, 99]
After sort[10, 20, 30, 50, 99
```

