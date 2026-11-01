# Tutorial 04 — Answers

## Question 1

### a.find the largest integer n so that n³ is less than 2000
```java
int n=0;
while((n*n*n)<2000){
    n++;
}
System.out.println("n= "+(n-1));
```

### b.display the square numbers of the first twelve integers starting from 1
```java
for (int i=1;i<=12;i++){
    System.out.println("Square of " + i + " is "+(i*i));
}
```

### c.display a 4-by-5 matrix using random numbers within 0 to 100
```java
Random r = new Random();
for(int row =1;row<=4;row++){
    for(int column=1;column<=5;column++){
        int num=r.nextInt(101);
        System.out.print(num+" ");
    }
    System.out.println();
}
```

### d.compute the sum of numbers from 1 to a given number
```java
Scanner sc= new Scanner(System.in);
System.out.print("Enter a number: ");
int num=sc.nextInt();
int sum=0;
for(int i=1;i<=num;i++){
    sum +=i;
}
System.out.println("Sum: "+sum);
```

### e.ompute the sum of the series 1/25 + 2/24 + 3/23 + … + 25/1 in two decimal places.
```java
double sum=0;
for(int i=1;i<=25;i++){
    sum+=(double)i/(26-i);
}
System.out.printf("Sum = %.2f%n",sum);
```


## Question 2

### a.
```java
int sum=0;
for (int x = 10; x > 0; x--)
    sum += x;
```

### b.
```java
int x=0,y=0;
do{
    x += 2;
    y += x;
    System.out.println(x + " and " + y);
}while (x < 100);
```

### c.
```java
for (int x=1, y=20; x < y; x++, y-=2)
    System.out.println(x + " " + y);
```

### d.
```java
int i =1;
while(i<=10) {
    if (i==10)
        System.out.println("Program End");
    i++;
}
```

## Question 3
```java
int previous=1,current=1;
System.out.print(previous+" "+current);
for(int i=3;i<=10;i++){
    int next=previous+current;
    System.out.print(" "+next);
    previous=current;
    current=next;
}
System.out.println();
```

## Question 4
```java
Scanner sc=new Scanner(System.in);
System.out.print("Enter a string: ");
String str = sc.nextLine();
for (int i = str.length() - 1; i >= 0; i--) {
    System.out.print(str.charAt(i));
}
System.out.println();
```