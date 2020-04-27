<div class="_description"><p>Since Java strings are <a href="https://en.wikipedia.org/wiki/Immutable_object" rel="nofollow noreferrer">immutable</a>, all methods which manipulate a <code>String</code> will <strong>return a new <code>String</code> object</strong>.  They do not change the original <code>String</code>. This includes to substring and replacement methods that C and C++ programers would expect to mutate the target <code>String</code> object.</p>
<hr />
<p>Use a <a href="https://docs.oracle.com/javase/8/docs/api/index.html?java/lang/StringBuilder.html" rel="nofollow noreferrer"><code>StringBuilder</code></a> instead of <code>String</code> if you want to concatenate more than two <code>String</code> objects whose values cannot be determined at compile-time. This technique is more performant than creating new <code>String</code> objects and concatenating them because <code>StringBuilder</code> is mutable.</p>
<p><a href="https://docs.oracle.com/javase/8/docs/api/index.html?java/lang/StringBuffer.html" rel="nofollow noreferrer"><code>StringBuffer</code></a> can also be used to concatenate <code>String</code> objects.  However, this class is less performant because it is designed to be thread-safe, and acquires a mutex before each operation.  Since you almost never need thread-safety when concatenating strings, it is best to use <code>StringBuilder</code>.</p>
<p>If you can express a string concatenation as a single expression, then it is better to use the <code>+</code> operator.  The Java compiler will convert an expression containing <code>+</code> concatenations into an efficient sequence of operations using either <code>String.concat(...)</code> or <code>StringBuilder</code>.  The advice to use <code>StringBuilder</code> explicitly only applies when the concatenation involves a multiple expressions.</p>
<hr />
<p>Don't store sensitive information in strings. If someone is able to obtain a memory dump of your running application, then they will be able to find all of the existing <code>String</code> objects and read their contents.  This includes <code>String</code> objects that are unreachable and are awaiting garbage collection.  If this is a concern, you will need to wipe sensitive string data as soon as you are done with it.  You cannot do this with <code>String</code> objects since they are immutable.  Therefore, it is advisable to use a <code>char[]</code> objects to hold sensitive character data, and wipe them (e.g. overwrite them with <code>'\000'</code> characters) when you are done.</p>
<hr />
<p><strong>All</strong> <code>String</code> instances are created on the heap, even instances that correspond to string literals. The special thing about string literals is that the JVM ensures that all literals that are equal (i.e. that consists of the same characters) are represented by a single <code>String</code> object (this behavior is specified in JLS).
This is implemented by JVM class loaders.  When a class loader loads a class, it scans for string literals that are used in the class definition, each time it sees one, it checks if there is already a record in the string pool for this literal (using the literal as a key). If there is already an entry for the literal, the reference to a <code>String</code> instance stored as the pair for that literal is used. Otherwise, a new  <code>String</code> instance is created and a reference to the instance is stored for the literal (used as a key) in the string pool. (Also see <a href="https://en.wikipedia.org/wiki/String_interning" rel="nofollow noreferrer">string interning</a>).</p>
<p>The string pool is held in the Java heap, and is subject to normal garbage collection.</p>
<div class='version-specific' data-version-json='[{&quot;Type&quot;:&quot;LessThan&quot;,&quot;GroupName&quot;:null,&quot;VersionName&quot;:&quot;Java SE 7&quot;}]'><span class='version-row'><span class='version'><span class='version-constraint version-kind-lessthan'>Java SE 7</span></span></span><div class='version-specific-content'>
<p>In releases of Java before Java 7, the string pool was held in a special part of the heap known as &quot;PermGen&quot;.  This part was only collected occasionally.</p>
</div></div>
<div class='version-specific' data-version-json='[{&quot;Type&quot;:&quot;GreaterThanOrEqual&quot;,&quot;GroupName&quot;:null,&quot;VersionName&quot;:&quot;Java SE 7&quot;}]'><span class='version-row'><span class='version'><span class='version-constraint version-kind-greaterthanorequal'>Java SE 7</span></span></span><div class='version-specific-content'>
<p>In Java 7, the string pool was moved off from &quot;PermGen&quot;.</p>
</div></div>
<p>Note that string literals are implicitly reachable from any method that uses them.  This means that the corresponding <code>String</code> objects can only be garbage collected if the code itself is garbage collected.</p>
<hr />
<p>Up until Java 8, <code>String</code> objects are implemented as a UTF-16 char array (2 bytes per char). There is a proposal in Java 9 to implement <code>String</code> as a byte array with an encoding flag field to note if the string is encoded as bytes (LATIN-1) or chars (UTF-16).</p>

</div><div class="_item"><h2 class="_title">Comparing Strings</h2><div class="_content"><p>In order to compare Strings for equality, you should use the String object's <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#equals-java.lang.Object-" rel="nofollow noreferrer"><code>equals</code></a> or <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#equalsIgnoreCase-java.lang.String-" rel="nofollow noreferrer"><code>equalsIgnoreCase</code></a> methods.</p>
<p>For example, the following snippet will determine if the two instances of <a href="https://docs.oracle.com/javase/7/docs/api/java/lang/String.html" rel="nofollow noreferrer"><code>String</code></a> are equal on all characters:</p>
<pre><code>String firstString = &quot;Test123&quot;;
String secondString = &quot;Test&quot; + 123;

if (firstString.equals(secondString)) {
   // Both Strings have the same content.
}
</code></pre>
<p><a href="https://ideone.com/TjaYMR" rel="nofollow noreferrer">Live demo</a></p>
<p>This example will compare them, independent of their case:</p>
<pre><code>String firstString = &quot;Test123&quot;;
String secondString = &quot;TEST123&quot;;

if (firstString.equalsIgnoreCase(secondString)) {
    // Both Strings are equal, ignoring the case of the individual characters.
}
</code></pre>
<p><a href="https://ideone.com/XxKmM1" rel="nofollow noreferrer">Live demo</a></p>
<p><strong>Note that</strong> <code>equalsIgnoreCase</code> does not let you specify a <code>Locale</code>. For instance, if you compare the two words <code>&quot;Taki&quot;</code> and <code>&quot;TAKI&quot;</code> in English they are equal; however, in Turkish they are different (in Turkish, the lowercase <code>I</code> is <code>ı</code>). For cases like this, converting both strings to lowercase (or uppercase) with <code>Locale</code> and then comparing with <code>equals</code> is the solution.</p>
<pre><code>String firstString = &quot;Taki&quot;;
String secondString = &quot;TAKI&quot;;

System.out.println(firstString.equalsIgnoreCase(secondString)); //prints true

Locale locale = Locale.forLanguageTag(&quot;tr-TR&quot;);

System.out.println(firstString.toLowerCase(locale).equals(
                   secondString.toLowerCase(locale))); //prints false
</code></pre>
<p><a href="https://ideone.com/uWc348" rel="nofollow noreferrer">Live demo</a></p>
<hr />
<h1>Do not use the == operator to compare Strings</h1>
<p>Unless you can guarantee that all strings have been interned (see below), you <strong>should not</strong> use the <code>==</code> or <code>!=</code> operators to compare Strings.  These operators actually test references, and since multiple <code>String</code> objects can represent the same String, this is liable to give the wrong answer.</p>
<p>Instead, use the <code>String.equals(Object)</code> method, which will compare the String objects based on their values.  For a detailed explanation, please refer to <a class='doc-link' href="http://stackoverflow.com/documentation/java/4388/java-pitfalls/16290/pitfall-using-to-compare-strings">Pitfall: using == to compare strings</a>.</p>
<hr />
<h1>Comparing Strings in a switch statement</h1>
<div class='version-specific' data-version-json='[{&quot;Type&quot;:&quot;GreaterThanOrEqual&quot;,&quot;GroupName&quot;:null,&quot;VersionName&quot;:&quot;Java SE 7&quot;}]'><span class='version-row'><span class='version'><span class='version-constraint version-kind-greaterthanorequal'>Java SE 7</span></span></span><div class='version-specific-content'>
<p>As of Java 1.7, it is possible to compare a String variable to literals in a <code>switch</code> statement. Make sure that the String is not null, otherwise it will always throw a <a class='doc-link' href="http://stackoverflow.com/documentation/java/1003/nullpointerexception#t=201608020755368222531"><code>NullPointerException</code></a>. Values are compared using <code>String.equals</code>, i.e. case sensitive.</p>
<pre><code>String stringToSwitch = &quot;A&quot;;

switch (stringToSwitch) {
    case &quot;a&quot;:
        System.out.println(&quot;a&quot;);
        break;
    case &quot;A&quot;:
        System.out.println(&quot;A&quot;); //the code goes here
        break;
    case &quot;B&quot;:
        System.out.println(&quot;B&quot;);
        break;
    default:
        break;
}
</code></pre>
<p><a href="https://ideone.com/fbWBUR" rel="nofollow noreferrer">Live demo</a></p>
</div></div>
<h1>Comparing Strings with constant values</h1>
<p>When comparing a <code>String</code> to a constant value, you can put the constant value on the left side of <code>equals</code> to ensure that you won't get a <code>NullPointerException</code> if the other String is <code>null</code>.</p>
<pre><code>&quot;baz&quot;.equals(foo)
</code></pre>
<p>While <code>foo.equals(&quot;baz&quot;)</code> will throw a <code>NullPointerException</code> if <code>foo</code> is <code>null</code>,  <code>&quot;baz&quot;.equals(foo)</code> will evaluate to <code>false</code>.</p>
<div class='version-specific' data-version-json='[{&quot;Type&quot;:&quot;GreaterThanOrEqual&quot;,&quot;GroupName&quot;:null,&quot;VersionName&quot;:&quot;Java SE 7&quot;}]'><span class='version-row'><span class='version'><span class='version-constraint version-kind-greaterthanorequal'>Java SE 7</span></span></span><div class='version-specific-content'>
<p>A more readable alternative is to use <code>Objects.equals()</code>, which does a null check on both parameters: <code>Objects.equals(foo, &quot;baz&quot;)</code>.</p>
</div></div>
<p>(<strong>Note:</strong> It is debatable as to whether it is better to avoid <code>NullPointerExceptions</code> in general, or let them happen and then fix the root cause; see <a class='doc-link' href="http://stackoverflow.com/documentation/java/5680/java-pitfalls-nulls-and-nullpointerexception/20151/pitfall-making-good-unexpected-nulls">here</a> and <a class='doc-link' href="http://stackoverflow.com/documentation/java/5680/java-pitfalls-nulls-and-nullpointerexception/23490/pitfall-using-yoda-conditions-to-avoid-nullpointerexception">here</a>.  Certainly, calling the avoidance strategy &quot;best practice&quot; is not justifiable.)</p>
<h1>String orderings</h1>
<p>The <code>String</code> class implements <code>Comparable&lt;String&gt;</code> with the <code>String.compareTo</code> method (as described at the start of this example).  This makes the natural ordering of <code>String</code> objects case-sensitive order.  The <code>String</code> class provide a <code>Comparator&lt;String&gt;</code> constant called <code>CASE_INSENSITIVE_ORDER</code> suitable for case-insensitive sorting.</p>
<h1>Comparing with interned Strings</h1>
<p>The Java Language Specification (<a href="https://docs.oracle.com/javase/specs/jls/se8/html/jls-3.html#jls-3.10.5" rel="nofollow noreferrer">JLS 3.10.6</a>) states the following:</p>
<blockquote>
<p>&quot;Moreover, a string literal always refers to the same instance of class <code>String</code>. This is because string literals - or, more generally, strings that are the values of constant expressions - are <em>interned</em> so as to share unique instances, using the method <code>String.intern</code>.&quot;</p>
</blockquote>
<p>This means it is safe to compare references to two string <em>literals</em> using <code>==</code>.  Moreover, the same is true for references to <code>String</code> objects that have been produced using the <code>String.intern()</code> method.</p>
<p>For example:</p>
<pre><code>String strObj = new String(&quot;Hello!&quot;);
String str = &quot;Hello!&quot;;

// The two string references point two strings that are equal
if (strObj.equals(str)) {
    System.out.println(&quot;The strings are equal&quot;);
}

// The two string references do not point to the same object
if (strObj != str) {
    System.out.println(&quot;The strings are not the same object&quot;);
}

// If we intern a string that is equal to a given literal, the result is
// a string that has the same reference as the literal.
String internedStr = strObj.intern();

if (internedStr == str) {
    System.out.println(&quot;The interned string and the literal are the same object&quot;);
}
</code></pre>
<p>Behind the scenes, the interning mechanism maintains a hash table that contains all interned strings that are still <em>reachable</em>.  When you call <code>intern()</code> on a <code>String</code>, the method looks up the object in the hash table:</p>
<ul>
<li>If the string is found, then that value is returned as the interned string.</li>
<li>Otherwise, a copy of the string is added to the hash table and that string is returned as the interned string.</li>
</ul>
<p>It is possible to use interning to allow strings to be compared using <code>==</code>.  However, there are significant problems with doing this;
see <a class='doc-link' href="http://stackoverflow.com/documentation/java/5455/java-pitfalls-performance-issues/23991/pitfall-interning-strings-so-that-you-can-use-is-a-bad-idea#t=201610101338294726756">Pitfall - Interning strings so that you can use == is a bad idea</a> for details.   It is not recommended in most cases.</p>

</div><h2 class="_title">Changing the case of characters within a String</h2><div class="_content"><p>The <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html" rel="nofollow noreferrer"><code>String</code></a> type provides two methods for converting strings between upper case and lower case:</p>
<ul>
<li><a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#toUpperCase--" rel="nofollow noreferrer"><code>toUpperCase</code></a> to convert all characters to upper case</li>
<li><a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#toLowerCase--" rel="nofollow noreferrer"><code>toLowerCase</code></a> to convert all characters to lower case</li>
</ul>
<p>These methods both return the converted strings as new <code>String</code> instances: the original <code>String</code> objects are not modified because <code>String</code> is immutable in Java. See this for more on immutability : <a href="http://stackoverflow.com/questions/1552301/immutability-of-strings-in-java">Immutability of Strings in Java</a></p>
<pre><code>String string = &quot;This is a Random String&quot;;
String upper = string.toUpperCase();
String lower = string.toLowerCase();

System.out.println(string);   // prints &quot;This is a Random String&quot;
System.out.println(lower);    // prints &quot;this is a random string&quot;
System.out.println(upper);    // prints &quot;THIS IS A RANDOM STRING&quot;
</code></pre>
<p>Non-alphabetic characters, such as digits and punctuation marks, are unaffected by these methods. Note that these methods may also incorrectly deal with certain Unicode characters under certain conditions.</p>
<hr />
<p><strong>Note</strong>: These methods are <em>locale-sensitive</em>, and may produce unexpected results if used on strings that are intended to be interpreted independent of the locale. Examples are programming language identifiers, protocol keys, and <code>HTML</code> tags.</p>
<p>For instance, <code>&quot;TITLE&quot;.toLowerCase()</code> in a Turkish locale returns &quot;<code>tıtle</code>&quot;, where <code>ı (\u0131)</code> is the <a href="http://www.fileformat.info/info/unicode/char/0131/index.htm" rel="nofollow noreferrer">LATIN SMALL LETTER DOTLESS I</a> character. To obtain correct results for locale insensitive strings, pass <code>Locale.ROOT</code> as a parameter to the corresponding case converting method (e.g. <code>toLowerCase(Locale.ROOT)</code> or <code>toUpperCase(Locale.ROOT)</code>).</p>
<p>Although using <code>Locale.ENGLISH</code> is also correct for most cases, the <strong>language invariant</strong> way is <code>Locale.ROOT</code>.</p>
<p>A detailed list of Unicode characters that require special casing can be found <a href="http://unicode.org/Public/UNIDATA/SpecialCasing.txt" rel="nofollow noreferrer">on the Unicode Consortium website</a>.</p>
<p><strong>Changing case of a specific character within an ASCII string:</strong></p>
<p>To change the case of a specific character of an ASCII string following algorithm can be used:</p>
<p>Steps:</p>
<ol>
<li>Declare a string.</li>
<li>Input the string.</li>
<li>Convert the string into a character array.</li>
<li>Input the character that is to be searched.</li>
<li>Search for the character into the character array.</li>
<li>If found,check if the character is lowercase or uppercase.
<ul>
<li>If Uppercase, add 32 to the ASCII code of the character.</li>
<li>If Lowercase, subtract 32 from the ASCII code of the character.</li>
</ul>
</li>
<li>Change the original character from the Character array.</li>
<li>Convert the character array back into the string.</li>
</ol>
<p>Voila, the Case of the character is changed.</p>
<p>An example of the code for the algorithm is:</p>
<pre><code>Scanner scanner = new Scanner(System.in);
System.out.println(&quot;Enter the String&quot;);
String s = scanner.next();
char[] a = s.toCharArray();
System.out.println(&quot;Enter the character you are looking for&quot;);
System.out.println(s);
String c = scanner.next();
char d = c.charAt(0);

for (int i = 0; i &lt;= s.length(); i++) {
    if (a[i] == d) {
        if (d &gt;= 'a' &amp;&amp; d &lt;= 'z') {
            d -= 32;
        } else if (d &gt;= 'A' &amp;&amp; d &lt;= 'Z') {
            d += 32;
        }
        a[i] = d;
        break;
    }
}
s = String.valueOf(a);
System.out.println(s);
</code></pre>

</div><h2 class="_title">Finding a String Within Another String</h2><div class="_content"><p>To check whether a particular String <code>a</code> is being contained in a String <code>b</code> or not, we can use the method <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#contains-java.lang.CharSequence-" rel="nofollow"><code>String.contains()</code></a> with the following syntax:</p>
<pre><code>b.contains(a); // Return true if a is contained in b, false otherwise
</code></pre>
<p>The <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#contains-java.lang.CharSequence-" rel="nofollow"><code>String.contains()</code></a> method can be used to verify if a <code>CharSequence</code> can be found in the String. The method looks for the String <code>a</code> in the String <code>b</code> in a case-sensitive way.</p>
<pre><code>String str1 = &quot;Hello World&quot;;
String str2 = &quot;Hello&quot;;
String str3 = &quot;helLO&quot;;

System.out.println(str1.contains(str2)); //prints true
System.out.println(str1.contains(str3)); //prints false
</code></pre>
<p><a href="https://ideone.com/Tdef6b" rel="nofollow">Live Demo on Ideone</a></p>
<hr />
<p>To find the exact position where a String starts within another String, use <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#indexOf-java.lang.String-" rel="nofollow"><code>String.indexOf()</code></a>:</p>
<pre><code>String s = &quot;this is a long sentence&quot;;
int i = s.indexOf('i');    // the first 'i' in String is at index 2
int j = s.indexOf(&quot;long&quot;); // the index of the first occurrence of &quot;long&quot; in s is 10
int k = s.indexOf('z');    // k is -1 because 'z' was not found in String s
int h = s.indexOf(&quot;LoNg&quot;); // h is -1 because &quot;LoNg&quot; was not found in String s
</code></pre>
<p><a href="https://ideone.com/RHHcF0" rel="nofollow">Live Demo on Ideone</a></p>
<p>The <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#indexOf-java.lang.String-" rel="nofollow"><code>String.indexOf()</code></a> method returns the first index of a <code>char</code> or <code>String</code> in another <code>String</code>. The method returns <code>-1</code> if it is not found.</p>
<p><strong>Note</strong>: The <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#indexOf-java.lang.String-" rel="nofollow"><code>String.indexOf()</code></a> method is case sensitive.</p>
<p>Example of search ignoring the case:</p>
<pre><code>String str1 = &quot;Hello World&quot;;
String str2 = &quot;wOr&quot;;
str1.indexOf(str2);                               // -1
str1.toLowerCase().contains(str2.toLowerCase());  // true
str1.toLowerCase().indexOf(str2.toLowerCase());   // 6
</code></pre>
<p><a href="https://ideone.com/TQtcMf" rel="nofollow">Live Demo on Ideone</a></p>

</div><h2 class="_title">Getting the length of a String</h2><div class="_content"><p>In order to get the length of a <code>String</code> object, call the <code>length()</code> method on it.
The length is equal to the number of UTF-16 code units (chars) in the string.</p>
<pre><code>String str = &quot;Hello, World!&quot;;
System.out.println(str.length()); // Prints out 13
</code></pre>
<p><a href="https://ideone.com/0RWKcA" rel="nofollow noreferrer">Live Demo on Ideone</a></p>
<p>A <code>char</code> in a String is UTF-16 value.  Unicode codepoints whose values are ≥ 0x1000 (for example, most emojis) use two char positions.  To count the number of Unicode codepoints in a String, regardless of whether each codepoint fits in a UTF-16 <code>char</code> value, you can use the <code>codePointCount</code> method:</p>
<pre><code>int length = str.codePointCount(0, str.length());
</code></pre>
<p>You can also use a Stream of codepoints, as of Java 8:</p>
<pre><code>int length = str.codePoints().count();
</code></pre>

</div><h2 class="_title">Substrings</h2><div class="_content"><pre><code>String s = &quot;this is an example&quot;;
String a = s.substring(11); // a will hold the string starting at character 11 until the end (&quot;example&quot;)
String b = s.substring(5, 10); // b will hold the string starting at character 5 and ending right before character 10 (&quot;is an&quot;)
String b = s.substring(5, b.length()-3); // b will hold the string starting at character 5 ending right before b' s lenght is out of 3  (&quot;is an exam&quot;)
</code></pre>
<p>Substrings may also be applied to slice and add/replace character into its original String. For instance, you faced a Chinese date containing Chinese characters but you want to store it as a well format Date String.</p>
<pre><code>String datestring = &quot;2015年11月17日&quot;
datestring = datestring.substring(0, 4) + &quot;-&quot; + datestring.substring(5,7) + &quot;-&quot; + datestring.substring(8,10);
//Result will be 2015-11-17
</code></pre>
<p>The <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#substring-int-" rel="nofollow noreferrer">substring</a> method extracts a piece of a <code>String</code>. When provided one parameter, the parameter is the start and the piece extends until the end of the <code>String</code>. When given two parameters, the first parameter is the starting character and the second parameter is the index of the character right after the end (the character at the index is not included). An easy way to check is the subtraction of the first parameter from the second should yield the expected length of the string.</p>
<div class='version-specific' data-version-json='[{&quot;Type&quot;:&quot;LessThan&quot;,&quot;GroupName&quot;:null,&quot;VersionName&quot;:&quot;Java SE 7&quot;}]'><span class='version-row'><span class='version'><span class='version-constraint version-kind-lessthan'>Java SE 7</span></span></span><div class='version-specific-content'>
<p>In JDK &lt;7u6 versions the <code>substring</code> method instantiates a <code>String</code> that shares the same backing <code>char[]</code> as the original <code>String</code> and has the internal <code>offset</code> and <code>count</code> fields set to the result start and length.
Such sharing may cause memory leaks, that can be prevented by calling <code>new String(s.substring(...))</code> to force creation of a copy, after which the <code>char[]</code> can be garbage collected.</p>
</div></div>
<div class='version-specific' data-version-json='[{&quot;Type&quot;:&quot;GreaterThanOrEqual&quot;,&quot;GroupName&quot;:null,&quot;VersionName&quot;:&quot;Java SE 7&quot;}]'><span class='version-row'><span class='version'><span class='version-constraint version-kind-greaterthanorequal'>Java SE 7</span></span></span><div class='version-specific-content'>
<p>From JDK 7u6 the <code>substring</code> method always copies the entire underlying <code>char[]</code> array, making the complexity linear compared to the previous constant one but guaranteeing the absence of memory leaks at the same time.</p>
</div></div>

</div><h2 class="_title">Getting the nth character in a String</h2><div class="_content"><pre><code>String str = &quot;My String&quot;;

System.out.println(str.charAt(0)); // &quot;M&quot;
System.out.println(str.charAt(1)); // &quot;y&quot;
System.out.println(str.charAt(2)); // &quot; &quot;
System.out.println(str.charAt(str.length-1)); // Last character &quot;g&quot;
</code></pre>
<p>To get the nth character in a string, simply call <code>charAt(n)</code> on a <code>String</code>, where <code>n</code> is the index of the character you would like to retrieve</p>
<p><strong>NOTE:</strong> index <code>n</code> is starting at <code>0</code>, so the first element is at n=0.</p>

</div><h2 class="_title">Platform independent new line separator</h2><div class="_content"><p>Since the new line separator varies from platform to platform (e.g. <code>\n</code> on Unix-like systems or <code>\r\n</code> on Windows) it is often necessary to have a platform-independent way of accessing it. In Java it can be retrieved from a system property:</p>
<pre><code>System.getProperty(&quot;line.separator&quot;)
</code></pre>
<div class='version-specific' data-version-json='[{&quot;Type&quot;:&quot;GreaterThanOrEqual&quot;,&quot;GroupName&quot;:null,&quot;VersionName&quot;:&quot;Java SE 7&quot;}]'><span class='version-row'><span class='version'><span class='version-constraint version-kind-greaterthanorequal'>Java SE 7</span></span></span><div class='version-specific-content'>
<p>Because the new line separator is so commonly needed, from Java 7 on a shortcut method returning exactly the same result as the code above is available:</p>
<pre><code>System.lineSeparator()
</code></pre>
</div></div>
<p><strong>Note</strong>: Since it is very unlikely that the new line separator changes during the program's execution, it is a good idea to store it in in a static final variable instead of retrieving it from the system property every time it is needed.</p>
<p>When using <code>String.format</code>, use <code>%n</code> rather than <code>\n</code> or '\r\n' to output a platform independent new line separator.</p>
<pre><code>System.out.println(String.format('line 1: %s.%nline 2: %s%n', lines[0],lines[1]));
</code></pre>

</div><h2 class="_title">Adding toString() method for custom objects</h2><div class="_content"><p>Suppose you have defined the following <code>Person</code> class:</p>
<pre><code>public class Person {

    String name;
    int age;
    
    public Person (int age, String name) {
        this.age = age;
        this.name = name;
    }
}
</code></pre>
<p>If you instantiate a new <code>Person</code> object:</p>
<pre><code>Person person = new Person(25, &quot;John&quot;);
</code></pre>
<p>and later in your code you use the following statement in order to print the object:</p>
<pre><code>System.out.println(person.toString());
</code></pre>
<p><a href="https://ideone.com/tAl58G" rel="nofollow">Live Demo on Ideone</a></p>
<p>you'll get an output similar to the following:</p>
<pre><code>Person@7ab89d
</code></pre>
<p>This is the result of the implementation of the <code>toString()</code> method defined in the <code>Object</code> class, a superclass of <code>Person</code>. The documentation of <code>Object.toString()</code> states:</p>
<blockquote>
<p>The toString method for class Object returns a string consisting of the name of the class of which the object is an instance, the at-sign character `@', and the unsigned hexadecimal representation of the hash code of the object. In other words, this method returns a string equal to the value of:</p>
<pre><code>getClass().getName() + '@' + Integer.toHexString(hashCode())
</code></pre>
</blockquote>
<p>So, for meaningful output, you'll have to <strong>override</strong> the <code>toString()</code> method:</p>
<pre><code>@Override
public String toString() {
    return &quot;My name is &quot; + this.name + &quot; and my age is &quot; + this.age;
}
</code></pre>
<p>Now the output will be:</p>
<pre><code>My name is John and my age is 25
</code></pre>
<p>You can also write</p>
<pre><code>System.out.println(person);
</code></pre>
<p><a href="https://ideone.com/51al3w" rel="nofollow">Live Demo on Ideone</a></p>
<p>In fact, <code>println()</code> implicitly invokes the <code>toString</code> method on the object.</p>

</div><h2 class="_title">Splitting Strings</h2><div class="_content"><p>You can split a <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html" rel="nofollow noreferrer"><code>String</code></a> on a particular delimiting character or a <a class='doc-link' href="http://stackoverflow.com/documentation/regex/topics">Regular Expression</a>, you can use the <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#split-java.lang.String-" rel="nofollow noreferrer"><code>String.split()</code></a> method that has the following signature:</p>
<pre><code>public String[] split(String regex)
</code></pre>
<p>Note that delimiting character or regular expression gets removed from the resulting String Array.</p>
<p>Example using delimiting character:</p>
<pre><code>String lineFromCsvFile = &quot;Mickey;Bolton;12345;121216&quot;;
String[] dataCells = lineFromCsvFile.split(&quot;;&quot;);
// Result is dataCells = { &quot;Mickey&quot;, &quot;Bolton&quot;, &quot;12345&quot;, &quot;121216&quot;};
</code></pre>
<p>Example using regular expression:</p>
<pre><code>String lineFromInput = &quot;What    do you need    from me?&quot;;
String[] words = lineFromInput.split(&quot;\\s+&quot;); // one or more space chars
// Result is words = {&quot;What&quot;, &quot;do&quot;, &quot;you&quot;, &quot;need&quot;, &quot;from&quot;, &quot;me?&quot;};
</code></pre>
<p>You can even directly split a <code>String</code> literal:</p>
<pre><code>String[] firstNames = &quot;Mickey, Frank, Alicia, Tom&quot;.split(&quot;, &quot;);
// Result is firstNames = {&quot;Mickey&quot;, &quot;Frank&quot;, &quot;Alicia&quot;, &quot;Tom&quot;};
</code></pre>
<p><strong>Warning</strong>: Do not forget that the parameter is always treated as a regular expression.</p>
<pre><code>&quot;aaa.bbb&quot;.split(&quot;.&quot;); // This returns an empty array
</code></pre>
<p>In the previous example <code>.</code> is treated as the regular expression wildcard that matches any character, and since every character is a delimiter, the result is an empty array.</p>
<hr />
<p><strong>Splitting based on a delimiter which is a regex meta-character</strong></p>
<p>The following characters are considered special (aka meta-characters) in regex</p>
<pre><code>  &lt; &gt; - = ! ( ) [ ] { } \ ^ $ | ? * + . 
</code></pre>
<p>To split a string based on one of the above delimiters, you need to either <em>escape</em> them using <code>\\</code> or use <code>Pattern.quote()</code>:</p>
<ul>
<li>
<p>Using <code>Pattern.quote()</code>:</p>
<pre><code> String s = &quot;a|b|c&quot;;
 String regex = Pattern.quote(&quot;|&quot;);
 String[] arr = s.split(regex);
</code></pre>
</li>
<li>
<p>Escaping the special characters:</p>
<pre><code> String s = &quot;a|b|c&quot;;
 String[] arr = s.split(&quot;\\|&quot;);
</code></pre>
</li>
</ul>
<hr />
<p><strong>Split removes empty values</strong></p>
<p><code>split(delimiter)</code> by default removes trailing empty strings from result array. To turn this mechanism off we need to use overloaded version of <code>split(delimiter, limit)</code> with limit set to negative value like</p>
<pre><code>String[] split = data.split(&quot;\\|&quot;, -1);
</code></pre>
<p><code>split(regex)</code> internally returns result of <code>split(regex, 0)</code>.</p>
<p>The limit parameter controls the number of times the pattern is applied and therefore affects the length of the resulting array.<br />
If the limit <em>n</em> is greater than zero then the pattern will be applied at most <em>n - 1</em> times, the array's length will be no greater than <em>n</em>, and the array's last entry will contain all input beyond the last matched delimiter.<br />
If <em>n</em> is negative, then the pattern will be applied as many times as possible and the array can have any length.<br />
If <em>n</em> is zero then the pattern will be applied as many times as possible, the array can have any length, and trailing empty strings will be discarded.</p>
<hr />
<p><strong>Splitting with a <code>StringTokenizer</code></strong></p>
<p>Besides the <a class='doc-link' href="http://stackoverflow.com/documentation/regex/topics"><code>split()</code></a> method Strings can also be split using a <code>StringTokenizer</code>.</p>
<p><code>StringTokenizer</code> is even more restrictive than <code>String.split()</code>, and also a bit harder to use. It is essentially designed for pulling out tokens delimited by a fixed set of characters (given as a <code>String</code>). Each character will act as a separator. Because of this restriction, it's about twice as fast as <code>String.split()</code>.</p>
<p>Default set of characters are empty spaces (<code>\t\n\r\f</code>). The following example will print out each word separately.</p>
<pre><code>String str = &quot;the lazy fox jumped over the brown fence&quot;;
StringTokenizer tokenizer = new StringTokenizer(str);
while (tokenizer.hasMoreTokens()) {
    System.out.println(tokenizer.nextToken());
}
</code></pre>
<p>This will print out:</p>
<pre><code>the
lazy 
fox 
jumped 
over 
the 
brown 
fence
</code></pre>
<p>You can use different character sets for separation.</p>
<pre><code>String str = &quot;jumped over&quot;;
// In this case character `u` and `e` will be used as delimiters 
StringTokenizer tokenizer = new StringTokenizer(str, &quot;ue&quot;);
while (tokenizer.hasMoreTokens()) {
    System.out.println(tokenizer.nextToken());
}
</code></pre>
<p>This will print out:</p>
<pre><code>j
mp 
d ov
r
</code></pre>

</div><h2 class="_title">Joining Strings with a delimiter</h2><div class="_content"><div class='version-specific' data-version-json='[{&quot;Type&quot;:&quot;GreaterThanOrEqual&quot;,&quot;GroupName&quot;:null,&quot;VersionName&quot;:&quot;Java SE 8&quot;}]'><span class='version-row'><span class='version'><span class='version-constraint version-kind-greaterthanorequal'>Java SE 8</span></span></span><div class='version-specific-content'>
<p>An array of strings can be joined using the static method <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#join-java.lang.CharSequence-java.lang.CharSequence...-" rel="nofollow"><code>String.join()</code></a>:</p>
<pre><code>String[] elements = { &quot;foo&quot;, &quot;bar&quot;, &quot;foobar&quot; };
String singleString = String.join(&quot; + &quot;, elements);

System.out.println(singleString); // Prints &quot;foo + bar + foobar&quot;     
</code></pre>
<p>Similarly, there's an overloaded <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/String.html#join-java.lang.CharSequence-java.lang.Iterable-" rel="nofollow"><code>String.join()</code></a> method for <code>Iterable</code>s.</p>
<hr />
<p>To have a fine-grained control over joining, you may use <a href="https://docs.oracle.com/javase/8/docs/api/java/util/StringJoiner.html" rel="nofollow">StringJoiner</a> class:</p>
<pre><code>StringJoiner sj = new StringJoiner(&quot;, &quot;, &quot;[&quot;, &quot;]&quot;); 
    // The last two arguments are optional, 
    // they define prefix and suffix for the result string

sj.add(&quot;foo&quot;);
sj.add(&quot;bar&quot;);
sj.add(&quot;foobar&quot;);

System.out.println(sj); // Prints &quot;[foo, bar, foobar]&quot;
</code></pre>
<hr />
<p>To join a stream of strings, you may use the <a href="https://docs.oracle.com/javase/8/docs/api/java/util/stream/Collectors.html#joining-java.lang.CharSequence-" rel="nofollow">joining collector</a>:</p>
<pre><code>Stream&lt;String&gt; stringStream = Stream.of(&quot;foo&quot;, &quot;bar&quot;, &quot;foobar&quot;);
String joined = stringStream.collect(Collectors.joining(&quot;, &quot;));
System.out.println(joined); // Prints &quot;foo, bar, foobar&quot;
</code></pre>
<p>There's an option to define <a href="https://docs.oracle.com/javase/8/docs/api/java/util/stream/Collectors.html#joining-java.lang.CharSequence-java.lang.CharSequence-java.lang.CharSequence-" rel="nofollow">prefix and suffix</a> here as well:</p>
<pre><code>Stream&lt;String&gt; stringStream = Stream.of(&quot;foo&quot;, &quot;bar&quot;, &quot;foobar&quot;);
String joined = stringStream.collect(Collectors.joining(&quot;, &quot;, &quot;{&quot;, &quot;}&quot;));
System.out.println(joined); // Prints &quot;{foo, bar, foobar}&quot;
</code></pre>
</div></div>

</div><h2 class="_title">Reversing Strings</h2><div class="_content"><p>There are a couple ways you can reverse a string to make it backwards.</p>
<ol>
<li>
<p>StringBuilder/StringBuffer:</p>
<pre><code> String code = &quot;code&quot;;
 System.out.println(code);

 StringBuilder sb = new StringBuilder(code); 
 code = sb.reverse().toString();

 System.out.println(code);
</code></pre>
</li>
<li>
<p>Char array:</p>
<pre><code>String code = &quot;code&quot;;
System.out.println(code);

char[] array = code.toCharArray();
for (int index = 0, mirroredIndex = array.length - 1; index &lt; mirroredIndex; index++, mirroredIndex--) {
    char temp = array[index];
    array[index] = array[mirroredIndex];
    array[mirroredIndex] = temp;
}

// print reversed
System.out.println(new String(array));
</code></pre>
</li>
</ol>

</div><h2 class="_title">Counting occurrences of a substring or character in a string</h2><div class="_content"><p><code>countMatches</code> method from <a href="http://org.apache.commons.lang3.StringUtils" rel="nofollow">org.apache.commons.lang3.StringUtils</a> is typically used to count occurences of a substring or character in a <code>String</code>:</p>
<pre><code>import org.apache.commons.lang3.StringUtils;

String text = &quot;One fish, two fish, red fish, blue fish&quot;;

// count occurrences of a substring
String stringTarget = &quot;fish&quot;;
int stringOccurrences = StringUtils.countMatches(text, stringTarget); // 4

// count occurrences of a char
char charTarget = ',';
int charOccurrences = StringUtils.countMatches(text, charTarget); // 3
</code></pre>
<p>Otherwise for does the same with standard Java API's you could use Regular Expressions:</p>
<pre><code>import java.util.regex.Matcher;
import java.util.regex.Pattern;
 
String text = &quot;One fish, two fish, red fish, blue fish&quot;;
System.out.println(countStringInString(&quot;fish&quot;, text)); // prints 4
System.out.println(countStringInString(&quot;,&quot;, text)); // prints 3
 

public static int countStringInString(String search, String text) {
    Pattern pattern = Pattern.compile(search);
    Matcher matcher = pattern.matcher(text);
    
    int stringOccurrences = 0;
    while (matcher.find()) {
      stringOccurrences++;
    }
    return stringOccurrences;
}
</code></pre>

</div><h2 class="_title">String concatenation and StringBuilders</h2><div class="_content"><p>String concatenation can be performed using the <code>+</code> operator. For example:</p>
<pre><code>String s1 = &quot;a&quot;;
String s2 = &quot;b&quot;;
String s3 = &quot;c&quot;;
String s = s1 + s2 + s3; // abc
</code></pre>
<p>Normally a compiler implementation will perform the above concatenation using methods involving a <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/StringBuilder.html" rel="nofollow noreferrer"><code>StringBuilder</code></a> under the hood. When compiled, the code would look similar to the below:</p>
<pre><code>StringBuilder sb = new StringBuilder(&quot;a&quot;);
String s = sb.append(&quot;b&quot;).append(&quot;c&quot;).toString();
</code></pre>
<p><code>StringBuilder</code> has several overloaded methods for appending different types, for example, to append an <code>int</code> instead of a <code>String</code>. For example, an implementation can convert:</p>
<pre><code>String s1 = &quot;a&quot;;
String s2 = &quot;b&quot;;    
String s = s1 + s2 + 2; // ab2
</code></pre>
<p>to the following:</p>
<pre><code>StringBuilder sb = new StringBuilder(&quot;a&quot;);
String s = sb.append(&quot;b&quot;).append(2).toString();
</code></pre>
<p>The above examples illustrate a simple concatenation operation that is effectively done in a single place in the code. The concatenation involves a single instance of the <code>StringBuilder</code>. In some cases, a concatenation is carried out in a cumulative way such as in a loop:</p>
<pre><code>String result = &quot;&quot;;
for(int i = 0; i &lt; array.length; i++) {
    result += extractElement(array[i]);
}
return result;
</code></pre>
<p>In such cases, the compiler optimization is usually not applied, and each iteration will create a new <code>StringBuilder</code> object. This can be optimized by explicitly transforming the code to use a single <code>StringBuilder</code>:</p>
<pre><code>StringBuilder result = new StringBuilder();
for(int i = 0; i &lt; array.length; i++) {
    result.append(extractElement(array[i]));
}
return result.toString();
</code></pre>
<p>A <code>StringBuilder</code> will be initialized with an empty space of only 16 characters. If you know in advance that you will be building larger strings, it can be beneficial to initialize it with sufficient size in advance, so that the internal buffer does not need to be resized:</p>
<pre><code>StringBuilder buf = new StringBuilder(30); // Default is 16 characters
buf.append(&quot;0123456789&quot;);
buf.append(&quot;0123456789&quot;); // Would cause a reallocation of the internal buffer otherwise
String result = buf.toString(); // Produces a 20-chars copy of the string
</code></pre>
<p>If you are producing many strings, it is advisable to reuse <code>StringBuilder</code>s:</p>
<pre><code>StringBuilder buf = new StringBuilder(100);
for (int i = 0; i &lt; 100; i++) {
    buf.setLength(0); // Empty buffer
    buf.append(&quot;This is line &quot;).append(i).append('\n');
    outputfile.write(buf.toString());
}
</code></pre>
<p>If (and only if) multiple threads are writing to the <em>same</em> buffer, use <a href="https://docs.oracle.com/javase/7/docs/api/java/lang/StringBuffer.html" rel="nofollow noreferrer">StringBuffer</a>, which is a <code>synchronized</code> version of <code>StringBuilder</code>. But because usually only a single thread writes to a buffer, it is usually faster to use <code>StringBuilder</code> without synchronization.</p>
<p><strong>Using concat() method:</strong></p>
<pre><code>String string1 = &quot;Hello &quot;;
String string2 = &quot;world&quot;;
String string3 = string1.concat(string2);  // &quot;Hello world&quot;
</code></pre>
<p>This returns a new string that is string1 with string2 added to it at the end. You can also use the concat() method with string literals, as in:</p>
<pre><code>&quot;My name is &quot;.concat(&quot;Buyya&quot;);
</code></pre>

</div><h2 class="_title">Replacing parts of Strings</h2><div class="_content"><p>Two ways to replace: by regex or by exact match.</p>
<p><strong>Note:</strong> the original String object will be unchanged, the return value holds the changed String.</p>
<h2>Exact match</h2>
<h3>Replace single character with another single character:</h3>
<pre><code>String replace(char oldChar, char newChar) 
</code></pre>
<blockquote>
<p>Returns a new string resulting from replacing all occurrences of oldChar in this string with newChar.</p>
</blockquote>
<pre><code>String s = &quot;popcorn&quot;;
System.out.println(s.replace('p','W'));
</code></pre>
<p>Result:</p>
<pre><code>WoWcorn
</code></pre>
<h3>Replace sequence of characters with another sequence of characters:</h3>
<pre><code>String replace(CharSequence target, CharSequence replacement) 
</code></pre>
<blockquote>
<p>Replaces each substring of this string that matches the literal target sequence with the specified literal replacement sequence.</p>
</blockquote>
<pre><code>String s = &quot;metal petal et al.&quot;;
System.out.println(s.replace(&quot;etal&quot;,&quot;etallica&quot;));
</code></pre>
<p>Result:</p>
<pre><code>metallica petallica et al.
</code></pre>
<h2>Regex</h2>
<p><strong>Note</strong>: the grouping uses the <code>$</code> character to reference the groups, like <code>$1</code>.</p>
<h3>Replace all matches:</h3>
<pre><code>String replaceAll(String regex, String replacement) 
</code></pre>
<blockquote>
<p>Replaces each substring of this string that matches the given regular expression with the given replacement.</p>
</blockquote>
<pre><code>String s = &quot;spiral metal petal et al.&quot;;
System.out.println(s.replaceAll(&quot;(\\w*etal)&quot;,&quot;$1lica&quot;));
</code></pre>
<p>Result:</p>
<pre><code>spiral metallica petallica et al.
</code></pre>
<h3>Replace first match only:</h3>
<pre><code>String replaceFirst(String regex, String replacement) 
</code></pre>
<blockquote>
<p>Replaces the first substring of this string that matches the given regular expression with the given replacement</p>
</blockquote>
<pre><code>String s = &quot;spiral metal petal et al.&quot;;
System.out.println(s.replaceAll(&quot;(\\w*etal)&quot;,&quot;$1lica&quot;));
</code></pre>
<p>Result:</p>
<pre><code>spiral metallica petal et al.
</code></pre>

</div><h2 class="_title">Remove Whitespace from the Beginning and End of a String</h2><div class="_content"><p>The <a href="http://docs.oracle.com/javase/8/docs/api/java/lang/String.html#trim--" rel="nofollow"><code>trim()</code></a> method returns a new String with the leading and trailing whitespace removed.</p>
<pre><code>String s = new String(&quot;   Hello World!!  &quot;);
String t = s.trim();  // t = &quot;Hello World!!&quot;
</code></pre>
<p>If you <code>trim</code> a String that doesn't have any whitespace to remove, you will be returned the same String instance.</p>
<p>Note that the <a href="http://docs.oracle.com/javase/8/docs/api/java/lang/String.html#trim--" rel="nofollow"><code>trim()</code></a> method <a href="http://stackoverflow.com/q/1437933/2170192">has its own notion of whitespace</a>, which differs from the notion used by the <a href="http://docs.oracle.com/javase/8/docs/api/java/lang/Character.html#isWhitespace-char-" rel="nofollow"><code>Character.isWhitespace()</code></a> method:</p>
<ul>
<li>
<p>All ASCII control characters with codes <code>U+0000</code> to <code>U+0020</code> are considered whitespace and are removed by <code>trim()</code>. This includes <code>U+0020 'SPACE'</code>, <code>U+0009 'CHARACTER TABULATION'</code>, <code>U+000A 'LINE FEED'</code> and <code>U+000D 'CARRIAGE RETURN'</code> characters, but also the characters like <code>U+0007 'BELL'</code>.</p>
</li>
<li>
<p>Unicode whitespace like <code>U+00A0 'NO-BREAK SPACE'</code> or <code>U+2003 'EM SPACE'</code> are <em>not</em> recognized by <code>trim()</code>.</p>
</li>
</ul>

</div><h2 class="_title">String pool and heap storage</h2><div class="_content"><p>Like many Java objects, <strong>all</strong> <code>String</code> instances are created on the heap, even literals. When the JVM finds a <code>String</code> literal that has no equivalent reference in the heap, the JVM creates a corresponding <code>String</code> instance on the heap <strong>and</strong> it also stores a reference to the newly created <code>String</code> instance in the String pool. Any other references to the same <code>String</code> literal are replaced with the previously created <code>String</code> instance in the heap.</p>
<p>Let's look at the following example:</p>
<pre><code>class Strings
{
    public static void main (String[] args)
    {
        String a = &quot;alpha&quot;;
        String b = &quot;alpha&quot;;
        String c = new String(&quot;alpha&quot;);

        //All three strings are equivalent
        System.out.println(a.equals(b) &amp;&amp; b.equals(c));

        //Although only a and b reference the same heap object
        System.out.println(a == b);
        System.out.println(a != c);
        System.out.println(b != c);
    }
}
</code></pre>
<p>The output of the above is:</p>
<pre><code>true
true
true
true
</code></pre>
<p><img src="file:///android_asset/img/S8Ouk.png" alt="Diagram of Java Heap and String pool" />
When we use double quotes to create a String, it first looks for String with same value in the String pool, if found it just returns the reference else it creates a new String in the pool and then returns the reference.</p>
<p>However using new operator, we force String class to create a new String object in heap space. We can use intern() method to put it into the pool or refer to other String object from string pool having same value.</p>
<p>The String pool itself is also created on the heap.</p>
<div class='version-specific' data-version-json='[{&quot;Type&quot;:&quot;LessThan&quot;,&quot;GroupName&quot;:null,&quot;VersionName&quot;:&quot;Java SE 7&quot;}]'><span class='version-row'><span class='version'><span class='version-constraint version-kind-lessthan'>Java SE 7</span></span></span><div class='version-specific-content'>
<p>Before Java 7, <code>String</code> <strong>literals</strong> were stored in the runtime constant pool in the method area of <code>PermGen</code>, that had a fixed size.</p>
<p>The String pool also resided in <code>PermGen</code>.</p>
</div></div>
<div class='version-specific' data-version-json='[{&quot;Type&quot;:&quot;GreaterThanOrEqual&quot;,&quot;GroupName&quot;:null,&quot;VersionName&quot;:&quot;Java SE 7&quot;}]'><span class='version-row'><span class='version'><span class='version-constraint version-kind-greaterthanorequal'>Java SE 7</span></span></span><div class='version-specific-content'>
<p><a href="http://www.oracle.com/technetwork/java/javase/jdk7-relnotes-418459.html" rel="nofollow noreferrer">RFC: 6962931</a></p>
<blockquote>
<p>In JDK 7, interned strings are no longer allocated in the permanent generation of the Java heap, but are instead allocated in the main part of the Java heap (known as the young and old generations), along with the other objects created by the application. This change will result in more data residing in the main Java heap, and less data in the permanent generation, and thus may require heap sizes to be adjusted. Most applications will see only relatively small differences in heap usage due to this change, but larger applications that load many classes or make heavy use of the <code>String.intern()</code> method will see more significant differences.</p>
</blockquote>
</div></div>

</div><h2 class="_title">Case insensitive switch</h2><div class="_content"><div class='version-specific' data-version-json='[{&quot;Type&quot;:&quot;GreaterThanOrEqual&quot;,&quot;GroupName&quot;:null,&quot;VersionName&quot;:&quot;Java SE 7&quot;}]'><span class='version-row'><span class='version'><span class='version-constraint version-kind-greaterthanorequal'>Java SE 7</span></span></span><div class='version-specific-content'>
<p><code>switch</code> itself can not be parameterised to be case insensitive, but if absolutely required, can behave insensitive to the input string by using <code>toLowerCase()</code> or <code>toUpperCase</code>:</p>
<pre><code>switch (myString.toLowerCase()) {
     case &quot;case1&quot; :
        ...            
     break;
     case &quot;case2&quot; :
        ...            
     break;
}
</code></pre>
<p><strong>Beware</strong></p>
<ul>
<li><code>Locale</code> might affect how <a class='doc-link' href="http://stackoverflow.com/documentation/java/109/strings/515/changing-the-case-of-characters-within-a-string">changing cases happen</a>!</li>
<li>Care must be taken not to have any uppercase characters in the labels - those will never get executed!</li>
</ul>
</div></div>

</div></div>