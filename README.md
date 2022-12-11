# String-class-Method-in-java
String class Method in java


          import java.nio.charset.StandardCharsets;
          import java.util.Scanner;

          public class stringLibrary {
              public static void main (String[] args){
                  Scanner console = new Scanner(System.in);
                  //String Method.....
                  System.out.println("String Method....");
                  System.out.println("Enter a String");

                  // charAt() 	Returns the character at the specified index (position)

                  String demo = console.nextLine();
                  char charAt = demo.charAt(4);
                  System.out.println("charAt "+charAt);

                  //codePointAt() 	Returns the Unicode of the character at the specified index

                  int codepoint = demo.codePointAt(5);
                  System.out.println("codePointAt "+codepoint);

                  //codePointBefore() 	Returns the Unicode of the character before the specified index

                  int codePointbefore = demo.codePointBefore(4);

                  System.out.println("codePointbefore "+codePointbefore);

                  //codePointCount() 	Returns the number of Unicode values found in a string.

                  int codePointCount = demo.codePointCount(0,demo.length());

                  System.out.println("codePointCount " +codePointCount);

                  //compareTo() 	Compares two strings lexicographically

                  String demo2 = "I am Farhan";

                  int compareTo = demo.compareTo(demo2);

                  System.out.println("compareTo() "+ compareTo);

                  //compareToIgnoreCase() 	Compares two strings lexicographically, ignoring case differences

                  int compareToIgnoreCase = demo.compareToIgnoreCase(demo2);

                  System.out.println("compareToIgnoreCase "+ compareToIgnoreCase);

                  //concat() 	Appends a string to the end of another string

                  String concat = demo.concat(demo2);

                  System.out.println("concat: "+ concat +" ");

                  //contains() 	Checks whether a string contains a sequence of characters

                  boolean contains = demo.contains("a");

                  System.out.println("contain: "+contains);

                  //contentEquals() 	Checks whether a string contains the exact same sequence
                  // of characters of the specified CharSequence or StringBuffer

                  boolean contentEqual = demo.contentEquals("farhan");

                  System.out.println("contentEqual "+contentEqual);

                  //copyValueOf() 	Returns a String that represents the characters of the character array
                  char[] myStr1 = {'H', 'e', 'l', 'l', 'o'};

                  String myStr2 = "";

                  myStr2 = myStr2.copyValueOf(myStr1, 0, 4);

                  System.out.println("CopyValueOf :" + myStr2);

                  //endsWith() Checks whether a string ends with the specified character(s)

                  boolean endsWith= demo.endsWith("s");

                  System.out.println("endsWith: "+endsWith);

                  //equals() 	Compares two strings. Returns true if the strings are equal, and false if not

                  System.out.println("equals "+demo2.equals(demo));

                  //equalsIgnoreCase() 	Compares two strings, ignoring case considerations

                  System.out.println("equalsIgnoreCase() "+demo.equalsIgnoreCase(demo2));

                  //format() 	Returns a formatted string using the specified locale, format string, and arguments

                  System.out.println("format: "+ String.format(demo,"%s" ));

                  //getBytes() 	Encodes this String into a sequence of bytes using the named charset,
                  // storing the result into a new byte array

                  System.out.println("getBytes: "+ demo.getBytes(StandardCharsets.US_ASCII));

                  //getChars() 	Copies characters from a string to an array of chars.


                  char arry []=new char[10];
                  demo.getChars(0,10,arry,0);
                  System.out.println(arry);
                  for (int i = arry.length-1; i>=0;i--){
                      System.out.print(arry[i]);
                  }
                  System.out.println();

                  //hashCode() 	Returns the hash code of a string

                  System.out.println("hashCode: "+demo.hashCode());

                  //indexOf() 	Returns the position of the first found occurrence of specified characters in a string

                  System.out.println("Index of(): "+demo.indexOf("a"));

                  //intern() 	Returns the canonical representation for the string object
                  //memory Related!
                  System.out.println("intern(): "+demo.intern());

                  //isEmpty() 	Checks whether a string is empty or not

                  System.out.println("isEmpty(): "+ demo.isEmpty());

                  //lastIndexOf() 	Returns the position of the last found occurrence of specified characters in a string

                  System.out.println("lastIndex(): "+demo.lastIndexOf("Aziz"));

                  //length() 	Returns the length of a specified string

                  System.out.println("length(): "+ demo.length());

                  //matches() 	Searches a string for a match against a regular expression, and returns the matches

                  System.out.println("matches(): "+ demo.matches("Farhan Aziz"));

                  //offsetByCodePoints() 	Returns the index within this String that is offset from the given index by codePointOffset code points

                  System.out.println("offsetByCodePoints(): "+ demo.offsetByCodePoints(2,8));

                  //regionMatches() 	Tests if two string regions are equal

                  System.out.println("regionMatches(): "+ demo.regionMatches(20,demo2,0,20));

                  //replace() Searches a string for a specified value,
                  // and returns a new string where the specified values are replaced

                  System.out.println("replace(): "+ demo.replace("a","r"));

                  //replaceFirst() 	Replaces the first occurrence of a substring that
                  // matches the given regular expression with the given replacement

                  System.out.println("replaceFirst(): "+ demo.replaceFirst("a","Genius"));

                  //replaceAll() 	Replaces each substring of this string that
                  // matches the given regular expression with the given replacement...

                  System.out.println("replaceAll(): "+ demo.replaceAll(demo,"Genius"));

                  //split() 	Splits a string into an array of substrings
                  String split[]= demo.split("a");
                  for (int i=0; i<split.length;i++){
                      System.out.println(split[i]);
                  }

                  //startsWith() 	Checks whether a string starts with specified characters

                  System.out.println("startWith(): "+demo.startsWith("f"));

                  //subSequence() 	Returns a new character sequence that is a subsequence of this sequence

                  System.out.println("subSequence(): "+ demo.subSequence(2,7));

                  //substring() 	Returns a new string which is the substring of a specified string

                  System.out.println("substring(): "+demo.substring(2));

                  //toCharArray() 	Converts this string to a new character array

                  char cdc[] = demo.toCharArray();
                  for (int i=0; i<cdc.length; i++){
                      System.out.print(cdc[i]);
                  }

                  //toLowerCase() Converts a string to lower case letters

                  System.out.println("toLowerCase(): "+ demo.toLowerCase());

                  //toString() 	Returns the value of a String object

                  System.out.println("toString(): "+demo.toString());

                  //toUpperCase() 	Converts a string to upper case letters

                  System.out.println("toUpperCase(): "+demo.toUpperCase());

                  //trim() Removes whitespace from both ends of a string

                  System.out.println("trim(): "+ demo.trim());

                  //valueOf() 	Returns the string representation of the specified value

                  System.out.println("valueOf(): "+ demo.valueOf(6));

              }
          }
