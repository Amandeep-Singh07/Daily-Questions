<img src="image3.png">

```

import java.util.Scanner;

public class Main {

public static void main(String[] args) {
    
    Scanner kash=new Scanner(System.in);
    
    int num=kash.nextInt();
    int arr[]=new int[num];
    
    
    for(int i=0;i<arr.length;i++){
        arr[i]=kash.nextInt();
    }
    
    for(int i=0;i<arr.length;i++){
        int sum=0;
        for(int j=i+1;j<arr.length;j++){
            sum+=arr[j];
        }
           if(arr[i]>sum){
               System.out.print(arr[i]+" ");
           }
            
        
    }
    
}
}

```








<img src="q5part1.png">
<img src="q5part2.png">

```

import java.util.Scanner;

class StringOps {
    // Method to reverse a single string
    public String manipulate(String[] input) {
        if (input.length == 1) {
            return reverse(input[0]);
        } else if (input.length == 2) {
            return concatenate(input[0], input[1]);
        } else {
            return "Invalid input";
        }
    }
    
    // Helper method to reverse a string
    private String reverse(String str) {
        StringBuilder reversed = new StringBuilder(str);
        return reversed.reverse().toString();
    }
    
    // Helper method to concatenate two strings
    private String concatenate(String str1, String str2) {
        return str1 + str2;
    }
}

class Main {
    public static void main(String[] args) {
        StringOps seetha = new StringOps();
        Scanner scanner = new Scanner(System.in);
        String input = scanner.nextLine().trim();
        String[] input_data = input.split(" ");
        String result = seetha.manipulate(input_data);
        System.out.println(result);
    }
}

```


