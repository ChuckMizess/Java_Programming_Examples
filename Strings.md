## Strings
* [How to compare two strings ?](#How to compare two strings)
* [How to search the last position of a substring ?](#How to search the last position of a substring ?)
* [How to remove a particular character from a string ?](#How to remove a particular character from a string ?)
* [How to replace a substring inside a string by another one ?](#How to replace a substring inside a string by another one ?)
* [How to reverse a String?](#How to reverse a String?)
* [How to search a word inside a string ?](#How)

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


