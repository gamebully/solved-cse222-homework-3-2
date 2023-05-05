Download Link: https://assignmentchef.com/product/solved-cse222-homework-3-2
<br>
<strong>Q1:</strong>

Implement a LinkedArrayList class which implements List interface and extends AbstractList class.

Your class should keep a linked list where each node contains an array of elements with constant capacity. These arrays should be partially filled arrays. Arrays in the nodes of the linked list, may contain different number of elements.

When you remove an element in the list, you should find the array containing the elements, first. During remove operation, you should shift the elements (coming after the removed element) in that array only. The other arrays should not be affected. Of course, if the number of elements in an array becomes zero, the node containing this array should also be removed from the linked list.

When you add a new element, you need to add the elements into the corresponding array. If the capacity of the array is exhausted, you should create a new node (containing an empty array) in the linked list instead of incrementing the size of the array (you are not allowed to reallocate). Of course, you may want to move some of the elements in the exhausted array into the new array.

You are not allowed to use any class in Collection hierarchy as a member. So, you need to define your own Node class to build a linked list and use basic array structure in Java. Note that you need to implement all required methods and ListIterator class.

Write a Main class to test each method in your class.

<strong>Q2:</strong>

Implement a SimpleTextEditor class which provides the some of the edit functionality of a text editor.

The text is represented by a list of characters in your class. Your class should include a Java List. Your class should provide the following methods:

<ul>

 <li>Read method to read in a text file and construct the text.</li>

 <li>Add method that adds one or more characters (given as a string) at the specified position (given as an integer index) in your text.</li>

 <li>Find method that returns the start index of the first occurrence of the searched group of characters.</li>

 <li>Replace method that replaces all occurrences of a character with another character. Write two implementations:</li>

</ul>

You have to write two versions of each method:

<ul>

 <li>by using the iterator (ListIterator) to navigate on the List</li>

 <li>without using the iterator, using simple for loop with index structure</li>

</ul>

So, there will be eight methods in total.

Write a Main class which:

<ul>

 <li>Tests each method of the SimpleTextEditor class.</li>

 <li>Measures the running time of your implementation for various text sizes.</li>

 <li>Creates a readable log file of the test.</li>

</ul>

Your should write a report for this question including the following

<ul>

 <li>Analysis of the performance of each method theoretically using the most appropriate asymptotic notation. Present the analysis for the following cases:</li>

</ul>

o List is an ArrayList and iterator is used o List is an ArrayList and iterator is not used o List is a LinkedList and iterator is used o List is a LinkedList and iterator is not used

<ul>

 <li>Comparison of the experimental performance of each operation when o List is an ArrayList and iterator is used o List is an ArrayList and iterator is not used o List is a LinkedList and iterator is used o List is a LinkedList and iterator is not used</li>

</ul>




<strong>Q3:</strong>

(Optional for extra credit) Implement a WordLinkedList class to handle words of a crossword puzzle.

Each node keeps a character and references to previous and next nodes. To link the words, each node may have a reference to a cross node, as well. Cross node reference for the character ‘U’ in the word “PUZZLES” is the reference of the node containing the character ‘U’ in the word “FUN”

<strong> </strong>




Your class will include following methods:

<ul>

 <li>The constructor which gets a string and constructs itself as WordLinkedList.</li>

 <li>Add cross method that adds a cross between itself and another word at specified indexes. Note that the other word should have the corresponding cross, as well.</li>

 <li>Remove cross method that removes a cross at specified index.</li>

 <li>Print method that prints the word, its cross words and cross indexes</li>

</ul>

Implement a CrossWordPuzzle class. Your class will have a list of WordLinkedList and following methods:

<ul>

 <li>Add word method that adds a word to the puzzle and its crosses if specified</li>

 <li>Remove word method that removes a word from the puzzle and its crosses</li>

 <li>Print method that prints each word in the puzzle with its cross words and indexes</li>

</ul>

Write a Main class where the user can add/remove words and print the puzzle words with their cross words and indexes