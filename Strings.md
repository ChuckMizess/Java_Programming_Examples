## Strings
* [How to compare two strings ?](#How to compare two strings)
* [How to search the last position of a substring ?](#How to search the last position of a substring ?)

### How to compare two strings
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
    
### How to search the last position of a substring ?
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
