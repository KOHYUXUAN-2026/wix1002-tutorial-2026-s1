# Tutorial 03 — Answers

## Question 1

### a.
```java
boolean result= 3*8==27;
System.out.println(result);
```

### b.
```java
if(num%2==0)
    System.out.println(num+ " is an even number.");
else
    System.out.println(num+ " is an odd number.");
```

### c.
```java
if(ch>='A' && ch<='Z')
    System.out.println(ch+ " is a capital letter.");
else
    System.out.println(ch+ " is not a capital letter.");
```

### d.
```java
if(s1.compareToIgnoreCase(s2)<=0)
    System.out.println(s1+" "+s2);
else
    System.out.println(s2+" "+s1);
```

### e.
```java
String day = switch(num){
    case 0 -> "Sunday";
    case 1 -> "Monday";
    case 2 -> "Tuesday";
    case 3 -> "Wednesday";
    case 4 -> "Thursday";
    case 5 -> "Friday";
    case 6 -> "Saturday";
    default -> "Invalid day";
};
System.out.println(day);
```

## Question 2

### a.
```java
if(num1==num2)
    System.out.println("Number 1 is equal to number 2.");
```

### b.
```java
if(x>y && x>z)
    System.out.println("x is the largest number");
```

### c.
```java
String s1 = "java", s2 = "java";
if(s1.equals(s2))
    System.out.println("They are equal strings.");
else
    System.out.println("They are not equal strings.");
```

### d.
```java
if (x>0 || y>0)
 System.out.println("Either x or y is positive");
```

## Question 3

### a.
```text
#####
$$$$$
```

### b.
```text
#####
$$$$$
```

### c.
```text
#####
```

### d.
```text
(no output)
```

## Question 4
```java
if(a>=b && a>=c)
    System.out.println(a+ " is the biggest number.");
else if(b>=c)
    System.out.println(b+ " is the biggest number.");
else
    System.out.println(c+ " is the biggest number.");
```

## Question 5
```java
if (year%400 ==0)
    System.out.println(year+ " is a leap year.");
else if (year%4==0 && year%100!=0)
    System.out.println(year+ " is a leap year.");
else
    System.out.println(year+ " is not a leap year.");
```