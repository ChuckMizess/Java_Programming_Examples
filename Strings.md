###Index
* [How to compare two strings ?](#How to compare two strings)
* [How to search the last position of a substring ?](#How to search the last position of a substring ?)
* [How to remove a particular character from a string ?](#How to remove a particular character from a string ?)
* [How to replace a substring inside a string by another one ?](#How to replace a substring inside a string by another one ?)
* [How to reverse a String?](#How to reverse a String?)
* [How to search a word inside a string ?](#How to search a word inside a string ?)
* [How to split a string into a number of substrings ?](#How to split a string into a number of substrings ?)
* [How to convert a string totally into upper case?](#How to convert a string totally into upper case?)
* [How to match regions in strings?](#How to match regions in strings?)
* [How to compare performance of string creation ?](#How to compare performance of string creation ?)
* [How to optimize string creation ?](#How to optimize string creation ?)
* [How to format strings ?](#How to format strings ?)
* [How to optimize string concatenation ?](#How to optimize string concatenation ?)
* [How to determine the Unicode code point in string](#How-to-determine-the-Unicode-code-point-in-string)
* [How to buffer strings](#how-to-buffer-strings)

### How to compare two strings
```
public class StringCompareEmp{
   public static void main(String args[]){
      String str = "Hello World";
      String anotherString = "hello world";
      Object objStr = str;
      System.out.println( str.compareTo(anotherString) );
      System.out.println( str.compareToIgnoreCase(anotherString) );
      System.out.println( str.compareTo(objStr.toString()));
   }
}
```
    
### How to search the last position of a substring ?
```
public class SearchlastString {
  public static void main(String[] args) {
     String strOrig = "Hello world ,Hello Reader";
     int lastIndex = strOrig.lastIndexOf("Hello");
     if(lastIndex == - 1){
        System.out.println("Hello not found");
     }else{
        System.out.println("Last occurrence of Hello
        is at index "+ lastIndex);
     }
  }
}
```

### How to remove a particular character from a string ?
```
public class Main {
   public static void main(String args[]) {
      String str = "this is Java";
      System.out.println(removeCharAt(str, 3));
   }
   public static String removeCharAt(String s, int pos) {
      return s.substring(0, pos) + s.substring(pos + 1);
   }
}
```

### How to replace a substring inside a string by another one ?
```
public class StringReplaceEmp{
   public static void main(String args[]){
      String str="Hello World";
      System.out.println( str.replace( 'H','W' ) );
      System.out.println( str.replaceFirst("He", "Wa") );
      System.out.println( str.replaceAll("He", "Ha") );
   }
}
```

### How to reverse a String?
```
public class StringReverseExample{
   public static void main(String[] args){
      String string="abcdef";
      String reverse = new StringBuffer(string).
      reverse().toString();
      System.out.println("\nString before reverse:
      "+string);
      System.out.println("String after reverse:
      "+reverse);
   }
}
```

### How to search a word inside a string ?
```
public class SearchStringEmp{
   public static void main(String[] args) {
      String strOrig = "Hello readers";
      int intIndex = strOrig.indexOf("Hello");
      if(intIndex == - 1){
         System.out.println("Hello not found");
      }else{
         System.out.println("Found Hello at index "
         + intIndex);
      }
   }
}
```

### How to split a string into a number of substrings ?
```
public class JavaStringSplitEmp{
   public static void main(String args[]){
      String str = "jan-feb-march";
      String[] temp;
      String delimeter = "-";
      temp = str.split(delimeter);
      for(int i =0; i < temp.length ; i++){
         System.out.println(temp[i]);
         System.out.println("");
         str = "jan.feb.march";
         delimeter = "\\.";
         temp = str.split(delimeter);
      }
      for(int i =0; i < temp.length ; i++){
         System.out.println(temp[i]);
         System.out.println("");
         temp = str.split(delimeter,2);
         for(int j =0; j < temp.length ; j++){
            System.out.println(temp[j]);
         }
      }
   }
}
```

### How to convert a string totally into upper case?
```
public class StringToUpperCaseEmp {
   public static void main(String[] args) {
      String str = "string abc touppercase ";
      String strUpper = str.toUpperCase();
      System.out.println("Original String: " + str);
      System.out.println("String changed to upper case: "
      + strUpper);
   }
}
```

### How to match regions in strings?
```
public class StringRegionMatch{
   public static void main(String[] args){
      String first_str = "Welcome to Microsoft";
      String second_str = "I work with Microsoft";
      boolean match = first_str.
      regionMatches(11, second_str, 12, 9);
      System.out.println("first_str[11 -19] == "
      + "second_str[12 - 21]:-"+ match);
   }
}
```

### How to compare performance of string creation ?
```
public class StringComparePerformance{
   public static void main(String[] args){      
      long startTime = System.currentTimeMillis();
      for(int i=0;i<50000;i++){
         String s1 = "hello";
         String s2 = "hello"; 
      }
      long endTime = System.currentTimeMillis();
      System.out.println("Time taken for creation" 
      + " of String literals : "+ (endTime - startTime) 
      + " milli seconds" );       
      long startTime1 = System.currentTimeMillis();
      for(int i=0;i<50000;i++){
         String s3 = new String("hello");
         String s4 = new String("hello");
      }
      long endTime1 = System.currentTimeMillis();
      System.out.println("Time taken for creation" 
      + " of String objects : " + (endTime1 - startTime1)
      + " milli seconds");
   }
}
```

### How to optimize string creation ?
```
public class StringOptimization{
   public static void main(String[] args){
      String variables[] = new String[50000];	  
      for( int i=0;i <50000;i++){
         variables[i] = "s"+i;
      }
      long startTime0 = System.currentTimeMillis();
      for(int i=0;i<50000;i++){
         variables[i] = "hello";
      }
      long endTime0 = System.currentTimeMillis();
      System.out.println("Creation time" 
      + " of String literals : "+ (endTime0 - startTime0) 
      + " ms" );
      long startTime1 = System.currentTimeMillis();
      for(int i=0;i<50000;i++){
         variables[i] = new String("hello");
      }
      long endTime1 = System.currentTimeMillis();
      System.out.println("Creation time of" 
      + " String objects with 'new' key word : " 
      + (endTime1 - startTime1)
      + " ms");
      long startTime2 = System.currentTimeMillis();
      for(int i=0;i<50000;i++){
         variables[i] = new String("hello");
         variables[i] = variables[i].intern();		  
      }
      long endTime2 = System.currentTimeMillis();
      System.out.println("Creation time of" 
      + " String objects with intern(): " 
      + (endTime2 - startTime2)
      + " ms");
   }
}
```

### How to format strings ?
```
import java.util.*;

public class StringFormat{
   public static void main(String[] args){
      double e = Math.E;
      System.out.format("%f%n", e);
      System.out.format(Locale.GERMANY, "%-10.4f%n%n", e);
   }
}
```

### How to optimize string concatenation ?
```
public class StringConcatenate{
   public static void main(String[] args){
      long startTime = System.currentTimeMillis();
      for(int i=0;i<5000;i++){
         String result = "This is"
         + "testing the"
         + "difference"+ "between"
         + "String"+ "and"+ "StringBuffer";
      }
      long endTime = System.currentTimeMillis();
      System.out.println("Time taken for string" 
      + "concatenation using + operator : " 
      + (endTime - startTime)+ " ms");
      long startTime1 = System.currentTimeMillis();
      for(int i=0;i<5000;i++){
         StringBuffer result = new StringBuffer();
         result.append("This is");
         result.append("testing the");
         result.append("difference");
         result.append("between");
         result.append("String");
         result.append("and");
         result.append("StringBuffer");
      }
      long endTime1 = System.currentTimeMillis();
      System.out.println("Time taken for String concatenation" 
      + "using StringBuffer : "
      + (endTime1 - startTime1)+ " ms");
   }
}
```

### How to determine the Unicode code point in string
```
public class StringUniCode{
   public static void main(String[] args){
      String test_string="Welcome to TutorialsPoint";
      System.out.println("String under test is = "+test_string);
      System.out.println("Unicode code point at" 
      +" position 5 in the string is = "
      +  test_string.codePointBefore(5));
   }
}
```

###How to buffer strings
```
public class StringBuffer{
   public static void main(String[] args) {
      countTo_N_Improved();
   }
   private final static int MAX_LENGTH=30;
   private static String buffer = "";
   private static void emit(String nextChunk) {
      if(buffer.length() + nextChunk.length() > MAX_LENGTH) {
         System.out.println(buffer);
         buffer = "";  
      }
      buffer += nextChunk;
   }
   private static final int N=100;
   private static void countTo_N_Improved() {
      for (int count=2; count7lt;=N; count=count+2) {
         emit(" " + count);
      }
   }
}
```



