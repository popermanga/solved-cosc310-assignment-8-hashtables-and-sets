Download Link: https://assignmentchef.com/product/solved-cosc310-assignment-8-hashtables-and-sets
<br>
The objectives of this assignment are to:

<ul>

 <li>Gain further experience with using interfaces.</li>

 <li>Gain experience with implementations of a Hashtable.</li>

 <li>Gain experience using Sets.</li>

 <li>Gain further experience with dictionary applications.</li>

 <li>Continue to practice good programming techniques.</li>

</ul>

<h3>Task:</h3>

<strong>Step 1:</strong>

Provide a hash table implementation of a Dictionary (use the same interface as assignment 7).  You may chose linear probe (open addressing) or separate chaining to handle collisions.  You may use the hashCode() method built into Object and overridden in String to obtain your initial hash index.  You still need to modify the return from hashCode() to accommodate the size of the array in your hashtable.  <strong>You do not need to handle rehashing the table to handle the case where you run out of capacity</strong>.  Instead, choose an initial size of sufficient size.  <strong>Note:</strong> The order returned by the iterator will no longer be sorted.

<strong>Step 2:</strong>

Create a jUnit test program to thoroughly test your hashtable implementation of a Dictionary (<strong>make sure you test various test cases with delete</strong>).

<strong>Step 3: </strong>

Create a word index program (not in edu.iup.cosc310.util).  The word index program must open a text file passed to it on the command line.  Your program must process the text file identifying the set of unique words in the file and the page numbers on which each word occurs.  Separate words on spaces, commas, tabs, newlines, carriage returns, dash, slash, periods, semicolons, colons, quotes, parenthesis, and square brackets (i.e. split on “\W+”. A page is considered to be 50 lines and starts at page 1.

After processing all the words in the input text file, your word index program must print a list of all the found words, <strong>in sorted order</strong>, together with the list of page numbers where the words are found.  The page numbers must be in sorted order and each page number only is printed once for a given word.  Thus, <strong>you must use a Set</strong> for maintaining the list of page numbers.  You can use one of Java’s Set implementations.   The output is to be is sorted word order.  Thus when iterating over the keys, <strong>you will need to place the keys into List and then use Collections.sort to sort</strong> them.

<h3>Deliverables:</h3>

<ul>

 <li>zip file containing the sources and class files of your interface, hash table implementation, and word index program. The .zip file must be named [Your name]Asmt8.zip.</li>

 <li>File containing the captured output from running your test program.</li>

 <li>File containing the captured output from executing your word count program against sylabus.txt of assignment 7.</li>

</ul>




<h3>Bonus –</h3>

<ul>

 <li>Handle rehashing the table when the load factor reaches 50%. Have the initial size for the table be 11. Effectively double the size of the table and round up to the nearest prime number (you can hard code into an array the prime numbers that apply.  Make sure to test the code in Junit tests.</li>

</ul>


