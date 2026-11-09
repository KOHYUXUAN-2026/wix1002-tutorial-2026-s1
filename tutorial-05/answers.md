# Tutorial 05 — Answers

## Question 1

### a.Declare an array that used to store 12 floating point numbers.
```java
double[] num = new double[12];
```

### b. Initialize an array that used to store the value of A to E.
```java
char[] ch = {'A','B','C','D','E'};
```

### c.Declare an array that used to store 100 students name.
```java
String[] name = new String[100];
```

### d.Declare an array for a table with 6 rows 2 columns to store integer value.
```java
int[][] num = new int[6][2];
```

### e. Initialize an array with the following value:
```java
int[][] num = {
    {6,9},
    {2,5},
    {4,6}
};
```

### f. After initialize the array, modify the value of the above array to 
```java
num[1][1] = 4;
num[2][0] = 3;
num[2][1] = 7;
```

### g.Display all the values of an array name contact in separate lines.
```java 
for(int i=0; i<contact.length;i++){
    System.out.println(contact[i]);
}
```

## Question 2

### a.
```java
String[] code = {"AAA", "AAB", "AAC", "AAD"};
```

### b.
```java
int[] num = new int[10];
int sum = 0;
for(int k=0; k<num.length; k++)
 sum+=num[k];
```

### c.
```java
int[][] t = new int[3][];
t[1] = new int[3];
t[1][2] = 5;
```

### d.
```java
int i=3;
int[] score = new int[5];
score [1] = 78;
score[++i] = 100;
```

## Question 3
```java
 int[] marks = new int[5]; //create array with 5 elements
 int i = 0, j = 1;
 marks[i] = 12;//marks[0]=12
 marks[j] = marks[i] + 19;         //12+19=31, marks[1]=31
 marks[j-1] = marks[j] * marks [j];//marks[0]=31*31=961
 marks[j*3] = marks[i+1];          //marks[3]=marks[1]=31
 marks[++j] = marks[i]%5;          //marks[2]=marks[0]%5=961%5=1
 marks[2*j] = marks[j-1];          //because of ++j,now j is 2, marks[4]=marks[1]=31

answers: marks[0]=961
         marks[1]=31
         marks[2]=1
         marks[3]=31
         marks[4]=31
```

## Question 4
```java
int count =0;
for(int i=0;i<sentence.length;i++){
    if(sentence[i].equals("the")){
        count++;
    }
}
System.out.println("Number of occurences of the word \"the\" is "+count);
```

## Question 5-display the string array name sentence and each string element in reverse order. 
```java
for(int i = sentence.length-1; i>=0; i--){
    for(int j =sentence[i].length()-1; j>=0;j--){
        System.out.print(sentence[i].charAt(j));
    }
    System.out.println();
}
```

## Question 6 Write the statements that generate 1 random integer within 0 – 255. Convert the number to binary and store the bit into an 8 bit array. Then, display the binary number.
```java
Random r = new Random();
int num = r.nextInt(256);
int[] binary = new int[8];
for(int i =binary.length-1;i>=0;i--){
    binary[i]=num%2;
    num=num/2;
}

for(int i=0;i<binary.length;i++){
    System.out.print(binary[i]);
}
```