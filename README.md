# Personal-Library
codecademy freeform project

/*Like books? This program easily analyzes completed books in a small, personal library, and subsequently prints out the books that a user has fully read. Using Hashmap.*/

Upon completion, feel free to explore and add additional functionality to the Library.

import java.util.HashMap;
public class Library{
  public Library(){}
  public void getFinishedBooks(HashMap<String, Boolean> library) {
  	if(library.size() < 1) {
      System.out.println("Sorry, but your book list is empty!"); 
    }
  else { 
    for (String book: library.keySet()) {
      System.out.println(book);}
    }
   } 
 public static void main(String[] args) {
   HashMap<String, Boolean> myBooks = new HashMap<String, Boolean>();
   myBooks.put("Road Down The Funnel", true);
   myBooks.put("Rat: A Biology", false);
   myBooks.put("TimeIn", true);
   myBooks.put("3D Food Printing", false);
  
   Library myLibrary = new Library();
   myLibrary.getFinishedBooks(myBooks);
 }
}
