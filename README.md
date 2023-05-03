Download Link: https://assignmentchef.com/product/solved-cs314-specification-10-huffman-coding-and-compression-programming-assignment-10
<br>
<span style="font-size: large;"> The purposes of this assignment are:</span>

<ol>

 <li><span style="font-size: large;">to practice implementing data structures</span></li>

 <li><span style="font-size: large;">to <b><u>use</u></b> and build multiple data structures to solve an interesting problem</span></li>

</ol>

<strong>Restriction: You may not use the Java PriorityQueue class in any way on this assignment.</strong>

<b><span style="font-size: large;">Many, many thanks to Owen Astrachan of Duke University for allowing me to use and modify his version of this assignment.</span></b>

<hr>

<b><span style="font-size: large;">Preparation</span></b>

<ol>

 <li><span style="font-size: large;">Print the assignment page and the <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm&amp;source=gmail&amp;ust=1619291902553000&amp;usg=AFQjCNENNT12uHVQd0nE3FwUvh43Ock3_w">howto</a> page.</span></li>

 <li><span style="font-size: large;">Download the starter code by downloading the <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanSource.zip" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanSource.zip&amp;source=gmail&amp;ust=1619291902553000&amp;usg=AFQjCNGaJ3cnY1wb6XIjOtwF6kryjFn4rA">HuffmanSource.zip</a> file. </span></li>

 <li><span style="font-size: large;">Download the zip files <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/calgary.zip" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/calgary.zip&amp;source=gmail&amp;ust=1619291902553000&amp;usg=AFQjCNG4xsy01TUb_ojbB_h3H4W3RW-h9A">calgary</a>, <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/waterloo.zip" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/waterloo.zip&amp;source=gmail&amp;ust=1619291902553000&amp;usg=AFQjCNGbhHJJnaNhDzDflxLQrIhcM1dN2A">waterloo</a>, and <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/BooksAndHTML.zip" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/BooksAndHTML.zip&amp;source=gmail&amp;ust=1619291902553000&amp;usg=AFQjCNGscXgHl-ti40P_q_-kClTpIZpBZQ">BooksAndHTML</a>.</span></li>

 <li><span style="font-size: large;">Refer to<a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/doc/index.html" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/doc/index.html&amp;source=gmail&amp;ust=1619291902553000&amp;usg=AFQjCNEpOdfERu6jFncMwEnzQtia74fUjQ"> this page for the documentation</a> for the provided classes and starter code. </span></li>

 <li><span style="font-size: large;">Finally download the various test files from below to test your program.</span></li>

</ol>

<h3>Advice</h3>

<span style="font-size: large;">There is a lot to do. This is a complicated problem and program. Start early. Read the documentation for the provided classes and the how-to. </span>

<span style="font-size: large;">Because the compression scheme involves reading and writing in bits as opposed to a chars or Strings, the program can be hard to debug. In order to facilitate the design/code/debug cycle, you should take care to develop the program in an incremental fashion. If you try to write the whole program at once, it will be difficult to get a completely working program. <strong>Past students have suffered much pain and gnashing of teeth because they made an error in the code they wrote early, their PriorityQueue for example, didn’t test it, and spent HOURS trying to find the bug. </strong>The <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm#develop" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm%23develop&amp;source=gmail&amp;ust=1619291902553000&amp;usg=AFQjCNHsqOfCB8Ja37pLhweOqxpnBPkXjw">howto development section</a> has more information on incremental development.</span>

<span style="font-size: large;">I have also provided a few files the data portion only of a file as the characters ‘0’ and ‘1’ along with spaces as separator characters. These can be used to check part of your work.</span>

<span style="font-size: large;">Finally some students have suggested they understood the file format much better after doing the <strong><em>decoder</em></strong> first. Your mileage may vary, but doing the decoder may make doing the encoder easier. (I think it is simply whatever you do second, decoder or encoder, will be easier than what you do first.)</span>

Summary:

<span style="font-size: large;">Implement a program that performs Huffman coding and compression on files of any type by reading in the file a byte at a time and interpreting the bytes as ints. You are given a number of classes to start with. Your solution will use <b>many</b> different classes. </span><b><span style="font-size: large;">This is a difficult assignment. The hardest of the semester. I strongly urge you to work with a partner you know and trust AND to start early.</span></b>

<span style="font-size: large;">For a review of Huffman coding see the <a href="https://www.cs.utexas.edu/~scottm/cs314/handouts/slides/Topic20HuffmanCoding.pdf" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/handouts/slides/Topic20HuffmanCoding.pdf&amp;source=gmail&amp;ust=1619291902553000&amp;usg=AFQjCNG48vH9JpPArtg7AF6pHOY0Euy8mQ">class slides</a>. Note, your actual results will be <strong>different</strong> than the first example in the <b>middle of slides</b> because the period character will be before any of the other letters in the initial priority queue AND because the example does not show the PSEUDO – EOF character with a frequency of 1. </span>

<span style="font-size: large;">Your algorithm output shall match the example at the <b>end of the slides.</b></span>

<b><span style="font-size: large;">Background</span></b>

<span style="font-size: large;">There are many techniques used to compress digital data. This assignment implements the Huffman coding algorithm.</span>

The <span style="font-size: large;"><a href="https://en.wikipedia.org/wiki/MP3" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://en.wikipedia.org/wiki/MP3&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNGk5_4H6oBBLeIDWhYoQAcGWJu7pg">MP3</a> <a href="https://en.wikipedia.org/wiki/Codec" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://en.wikipedia.org/wiki/Codec&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNFNp9IGDSpuEDbKurZSpkdG1UYCLw">codec</a> <a href="http://www.mp3-converter.com/mp3codec/huffman_coding.htm" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://www.mp3-converter.com/mp3codec/huffman_coding.htm&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNEsAbgxxxDG9UdyCb5ufnkA_xbLjQ">uses Huffman encoding as one of the steps of the algorithm</a>.</span>

<span style="font-size: large;">Huffman coding was invented by David Huffman while he was a graduate student at MIT in 1950 when given the option of a term paper or a final exam. For details <a href="http://www.huffmancoding.com/my-uncle/scientific-american" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://www.huffmancoding.com/my-uncle/scientific-american&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNGqAFT6_N6yF5DQZEXcOmtDEvCpwA">see this 1991 Scientific American Article</a>. In an autobiography Huffman had this to say about the epiphany that led to his invention of the coding method that bears his name: </span>

<blockquote>

 <em><span style="font-size: large;">“– but a week before the end of the term I seemed to have nothing to show for weeks of effort. I knew I’d better get busy fast, do the standard final, and forget the research problem. I remember, after breakfast that morning, throwing my research notes in the wastebasket. And at that very moment, I had a sense of sudden release, so that I could see a simple pattern in what I had been doing, that I hadn’t been able to see at all until then. The result is the thing for which I’m probably best known: the Huffman Coding Procedure. I’ve had many breakthroughs since then, but never again all at once, like that. It was very exciting.” </span></em>

</blockquote>

<span style="font-size: large;"><a href="https://tinyurl.com/pckpeth" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://tinyurl.com/pckpeth&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNFO54PwyCbffEsIX-8DLaj8paBeog">Huffman’s original paper</a> is available, though it’s a tough read. <a href="https://en.wikipedia.org/wiki/Huffman_coding" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://en.wikipedia.org/wiki/Huffman_coding&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNHEkF3a8t5X8TbQgK8DfN-zeGj4DQ">The Wikipedia reference</a> is extensive as is this online material developed as one of the original <a href="http://nifty.stanford.edu/" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://nifty.stanford.edu/&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNHFb3uBEPIP_Q120CgoglHB6uva6A">Nifty Assignments</a>. Both jpeg and mp3 encodings use Huffman Coding as part of their compression algorithms. In this assignment you’ll implement a program to encode and decode files using a Huffman coding algorithm, hopefully resulting in a smaller, compressed file.</span>

<hr>

<h2><span style="font-size: large;">Assignment Overview</span></h2>

<span style="font-size: large;">Build a program that performs two related tasks: compressing (huff) files and  uncompressing (unhuff) files that are compressed by the first part of the program. This is done via a single program with the choice of compressing a file or uncompressing a file specified by choosing a menu-option in the GUI front-end to the code you write. Abstractly you’re writing a program to read an input file and create a corresponding output file — either from uncompressed to compressed or <em>vice versa</em>. </span>

<span style="font-size: large;">The <code>Huff</code> class is a simple main that launches a GUI with a connected <code>IHuffProcessor</code> <wbr>implementation. The implementation corresponds to an object oriented model named the model-view architecture or pattern. In this pattern the view/GUI makes calls on the model/<code>IHuffProcessor</code> methods which in turn may display information in the view/GUI. The code you write will also create files of compressed or uncompressed data when the GUI-front end calls methods you will write. You’ll implement methods and store state in your <code>IHuffProcessor</code> <wbr>implementation so that it can either compress/huff or uncompress/unhuff. You should implement additional classes to break the problem up into smaller, more manageable pieces and prevent repeated code. You should have a class that models a Huffman code tree, and a priority queue. You may find it useful to have separate classes to manage the details of compression (<code>Compressor</code>) and decompression (<code>Decompress</code>). With these additional classes the <code>SimpleHuffProcessor</code>remains relatively small. </span>

<span style="font-size: large;">The  <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNFdFEj8VUD1jVMjqTQz0AaKxnQm5A">howto for this assignment</a> contains a lot of details and explanations.</span>

<span style="font-size: large;">The resulting program will be a complete and useful compression program although not, perhaps, as powerful as other programs such as <em>winrar</em> or <em>zip</em> which use different algorithms resulting in a higher degree of compression than Huffman coding. </span>

<b><span style="font-size: large;">Important Constraints: These will make more sense after you get going on the assignment. These constraints are necessary to test and grade your program.</span></b>

<ol>

 <li><b><span style="font-size: large;">When adding number / frequency pairs to your priority queue, you must add them in ascending order based on the number represented by the chunk of bits. In other words add 0 and the frequency of 0, 1 and the frequency of  1, and so forth for all frequencies greater than 0.</span></b></li>

 <li><b><b><span style="font-size: large;">Your priority queue must handle ties in priority in a <i>fair</i> way. This means when adding an item to the queue with a priority equal to other items in the queue, the new item must go behind the items already present.</span></b></b>Consider this example. The front of the queue is on the left and the back of the queue is on the right. An items priority is based on the integer shown. The lower the integer the higher the priority.<code>FRONT [[X, 1], [A, 6], [E, 6], [S, 10]] BACK</code>now enqueue [Y, 6]. This value must come after the [E, 6], but before the [S,10]resulting priority queue after enqueuing [Y, 6]FRONT [[X, 1], [A, 6], [E, 6], [Y, 6], [S, 10]] BACKThis means you cannot use the Java PriorityQueue class because it breaks ties in an arbitrary manner. When enqueue an element it may jump in front of elements already present in the queue with the same priority. You are restricted from using the Java PriorityQueue class in any way on this assignment. You must implement your own priority queue that breaks ties in a fair way meaning in the case of ties we go by the order elements are added to the queue, first in first out, last in last out.</li>

 <li><b><span style="font-size: large;">When dequeueing elements from the priority queue to build the Huffman code tree the first element dequeued must be the left child of the new node and the second element dequeued must be the right child of the new node.</span></b></li>

 <li><span style="font-size: large;"><b>Do NOT rely on <a href="https://docs.oracle.com/javase/7/docs/api/java/io/InputStream.html#reset%28%29" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://docs.oracle.com/javase/7/docs/api/java/io/InputStream.html%23reset%2528%2529&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNEnYMBcKhrEe21r-ls8IF3tw4n_9g">the <code>reset</code> method from the Java <code>InputStream</code> class</a>. The test harness uses an <code>InputStream</code> that does not support that method and simply throws an exception. You will fail many, many tests if you rely on the Java <code>InputStream</code> <code>reset</code> method.</b></span></li>

</ol>

<hr>

<h2><span style="font-size: large;">The Huffman Compression Process</span></h2>

<span style="font-size: large;">The <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm#compress" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm%23compress&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNEZRcYvfvqVtSN5Uxrm4SQHFS4Zwg">Howto compression section</a> has complete information on how to create a compressed file. Create a Huffman tree to derive per-chunk encodings, then write bits based on these encodings. The <code>Huff</code> main program has a GUI front-end whose menu offers four choices: count chunk values, compress, uncompress, and quit as a fourth choice. </span>

<span style="font-size: large;">The count options in the GUI counts chunks, generates Huffman codes, and determines the number of bits in the resulting file if it were to be written using the new Huffman Codes determined by this method along with all required header data. This option does not actually write any data out to a new file. <b>Note, to determine the number of bits saved, the number of bits written includes ALL bits that will be written including the magic number, the header format number, the header to reproduce the tree, AND the actual data.</b></span>

<span style="font-size: large;">The compress option performs the same operations as the count characters option, but also writes the data out to a file. <b>Note, the compress option in the HuffViewer will first call the preprocess compress method BEFORE calling the compress method. </b></span>

<p dir="ltr"><span style="font-size: large;">Your <code>SimpleHuffProcessor</code> has a reference back to the <code>HuffViewer</code>. It shall  make calls to the <code>HuffViewer</code> <code>showError</code>, <code>show<wbr>Message</code>, and <code>update</code> methods to display the status, codes, and other information. Do not use <code>System.out.println</code>, use the methods from the <code>HuffViewer</code>.</span>

<ul>

 <li dir="ltr"><p dir="ltr"><span style="font-size: large;"><b>The <code>preprocessCompress</code> method must return the number of bits in the original file – the number of bits written to the compressed file (including the Huffman magic number, the header constant, the header, the data, and the pseudo-eof, but NOT any padding added by the file system to get the file size up to a multiple of 8.) </b></span></li>

 <li dir="ltr"><p dir="ltr"><span style="font-size: large;"><b>The <code>compress</code> method returns the number of bits actually written. It also writes out the compressed file using the codes generated from the previous call to preprocessCompress.</b></span></li>

 <li dir="ltr"><p dir="ltr"><span style="font-size: large;"><b>The <code>uncompress</code> method returns the number of bits written to the output file. It also uncompresses the compressed file.</b></span></li>

</ul>

<h2><span style="font-size: large;">The Huffman Decompression Process</span></h2>

<span style="font-size: large;">The uncompress option is used to decompress a file.</span>

<span style="font-size: large;">To uncompress a file your program previously compressed you’ll need to read <em>header information</em> from the compressed file your program (or other versions of the Huffman compressor) creates. The header information is data used to recreate the Huffman tree that was originally used to compress the data. Your code will then read one-bit-at-a-time to uncompress the data and recreate the original file. There’s information in the <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm#decompress" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm%23decompress&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNFt4OmJ8WwQHi2yQYoSyEyS0lXp_A">howto uncompress</a> section on doing this. </span>

<span style="font-size: large;">Read the header information to recreate the tree, then do a tree-walk one bit at a time to find the characters stored in the leaves of the Huffman tree. Each time you find a leaf, write the value to the output (and if debugging, to the <code>HuffView</code> GUI.). This process recreates the original, uncompressed file. </span>

<span style="font-size: large;">The uncompress option is used to decompress a file.</span>

<h2><span style="font-size: large;">Empirical Analysis</span></h2>

<span style="font-size: large;">Run the program <code>HuffMark</code> which will read every file in a directory and compress it to another file in the same directory with a <em>“.hf”</em> suffix. The <code>HuffMark</code> program does not provide a viewer for your <code>SimpleHuffProcessor</code> so you have to comment out any calls to <code>showString</code> or <code>viewer.<wbr>showMessage</code>. You can leave in the calls to <code>showError</code> assuming you won’t suffer any errors. The method calls may be in other classes if you created separate <code>Compressor</code> and <code>Decomp<wbr>ressor</code> classes. </span>

<span style="font-size: large;">You may want to modify this benchmarking program to print more data than it currently does, and to run it on the <em>calgary</em> directory which represents the <a href="http://corpus.canterbury.ac.nz/descriptions/#calgary" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://corpus.canterbury.ac.nz/descriptions/%23calgary&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNHm2Mz7xGKdp6q49uDNDGXWmvzdIQ">Calgary Corpus</a>, a standard compression suite of files for empirical analysis. <a href="http://www.data-compression.info/Comparisons/index.html" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://www.data-compression.info/Comparisons/index.html&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNH7oHeY6XxPjB7sr775KPJ1MRQoFg">See this reference for comparisons of the Calgary Corpus</a>, and the <em>waterloo</em> directory which is a collection of .tiff images used in some compression benchmarking, and on the <i>BooksAndHTML</i> directory which contains a number of text files and html documents. All of those collections are in zip files which you must download and unzip. You can, of course, run on other data/collections.</span>

<span style="font-size: large;">The benchmarking program skips files with <em>.hf</em> suffixes, but you may want to eventually remove this restriction . (In other words, what happens if you take a compressed file and try and compress it again?) In your assignment write-up discuss your benchmark results and provide some insight as to their meaning. <b>Your analysis is worth 15% of your grade on this assignment</b>, so you should try to come to some conclusions in addition to simply listing your results. </span>

<p dir="ltr"><b><span style="font-size: large;">Some Results From my version of the program.</span></b>

<ul>

 <li dir="ltr"><p dir="ltr"><span style="font-size: large;">This small sample file (that contains “Eerie eyes seen near lake.”) is 26 bytes or 208 bits. </span>

  <ul>

   <li dir="ltr"><p dir="ltr"><span style="font-size: large;">When I “compress” is with the <i>Standard Count Format Header</i> (see how-to document for explanation) the resulting size is 8346 bits. (The resulting file is 8352 bits, not 8346 bits. Why? 8346 is 1043.25 bytes. Or 1043 bytes and 2 bits. The file must be written as bytes so there are 6 bits of padding. This is the whole purpose of the pseudo-eof character. To know when the real data has ended and to ignore whatever padding may follow.)</span></li>

   <li dir="ltr"><p dir="ltr"><span style="font-size: large;">When I “compress” it with the <i>Standard Tree Format Header </i>the resulting size is 328 bits.</span></li>

  </ul></li>

 <li><p dir="ltr"><span style="font-size: large;">The <i>2008 CIA Factbook</i> is 9,637,228 bytes or 77,097,824 bits</span>

  <ul>

   <li dir="ltr"><p dir="ltr"><span style="font-size: large;">When I compress it with the <i>Standard Count Format Header</i> the compressed file is 48,230,392 bits.</span></li>

   <li dir="ltr"><p dir="ltr"><span style="font-size: large;">When I compress it with the <i>Standard Tree Format Header </i>the compressed file is 48,223,298 bits. </span></li>

  </ul></li>

</ul>

<p dir="ltr"><span style="font-size: large;">When I run HuffMark on the BooksAndHTML directory I get these results (Note, your times <strong>DO NOT</strong> have to be close to these.):</span>

<p dir="ltr"><span style="font-size: large;"><img decoding="async" class="CToWUd a6T" tabindex="0" src="https://ci6.googleusercontent.com/proxy/BJsTOvvKL-KC-nhAs7VS1gyf9ncl1YEf04Kb9ml0ghzRW5mKODFPH_x3v2vBugy7BbpRBBWF1gIZQFaJCCfsEY-DFWEInpQ=s0-d-e1-ft#https://www.cs.utexas.edu/~scottm/images/A11_Hu1.jpg" alt="HuffMark Output for Huffman Code / Compression assignments - CS314" border="0"></span>

<p dir="ltr"><span style="font-size: large;">My solution to the problem, which supports the standard count headers and the tree headers, consists of 4 classes in addition to the <code>SimpleHuffProcessor</code> with about 650 lines including code, blank lines, lines with single braces, and comments. (lots of comments)</span>

<p dir="ltr"><b><span style="font-size: large;">Resources</span></b>

<table border="1" width="100%" cellspacing="3" cellpadding="3">

 <tbody>

  <tr>

   <td align="right" width="15%" height="19"></td>

   <td width="70%" height="19"><span style="font-size: large;">File</span></td>

   <td width="15%" height="19"><span style="font-size: large;">Responsibility</span></td>

  </tr>

  <tr>

   <td align="right" width="15%" height="19"><span style="font-size: large;">Starter Code</span></td>

   <td width="70%" height="19"><span style="font-size: large;"><a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanSource.zip" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanSource.zip&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNHLilgKMXtTbBzKSbUg8OVO_DlOxA">HuffmanSource.zip </a>A zip file with the given classes to use in the assignment. You will make significant additions to <code>SimpleHuffProcessor</code>. Do not make any changes to the other given classes or interfaces.</span></td>

   <td width="15%" height="19"><span style="font-size: large;">Provided by me and you</span></td>

  </tr>

  <tr>

   <td align="right" width="15%" height="19"><span style="font-size: large;">Guide</span></td>

   <td width="70%" height="19"><span style="font-size: large;">The <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/HuffmanHowTo.htm&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNFdFEj8VUD1jVMjqTQz0AaKxnQm5A">Huffman HOWTO page</a> is a guide to help you complete the assignment. It gives an overview of the various parts of the assignment. And a <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/about_huff_compressed_file.pdf" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/about_huff_compressed_file.pdf&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNFCRrMsT5h_Xrhm3YSctvdy9fpawA">second howto</a> written by a TA, Claire. (Here is the <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/Claire_Howto_Alt.pdf" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/Claire_Howto_Alt.pdf&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNEFpVmQTntMhmy0uDbzDe6xHeHFdA">original, hand written version</a> which I think is charming.)</span></td>

   <td width="15%" height="19"><span style="font-size: large;">Provided by me</span></td>

  </tr>

  <tr>

   <td align="right" width="15%" height="19"><span style="font-size: large;">Documentation</span></td>

   <td width="70%" height="19"><a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/doc/index.html" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/doc/index.html&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNEf29AdgWAfqnog1imUlXpxV5GWkQ"><span style="font-size: large;">Documentation</span></a><span style="font-size: large;"> for the provided, non standard Java classes. You will have to refer to the documentation a great deal.</span></td>

   <td width="15%" height="19"><span style="font-size: large;">Provided by me</span></td>

  </tr>

  <tr>

   <td align="right" width="15%" height="19"><span style="font-size: large;">Small Test File</span></td>

   <td width="70%" height="19"><span style="font-size: large;">The small text file contains “Eerie eyes seen near lake.”</span><a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/smallTxt.txt" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/smallTxt.txt&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNGJ5y1yL0mpInuxzBICi8ctuWkrSg"><span style="font-size: large;">s</span></a><span style="font-size: large;"><a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/smallTxt.txt" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/smallTxt.txt&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNGJ5y1yL0mpInuxzBICi8ctuWkrSg">mallTxt.txt</a>, <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/smallTxtCountHeader.txt.hf" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/smallTxtCountHeader.txt.hf&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNG0P-X64R7ThsIpqxn227QuOSDKrA">SmallTxtCountHea<wbr>der.txt.hf</a>, and <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/smallTxtTreeHeader.txt.hf" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/smallTxtTreeHeader.txt.hf&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNGfeTUGxHIaPJ8C2nb7ePaPUd2W7g">SmallTxtTreeHeader.txt.hf</a>. Small sample file to use when incrementally developing your program. <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/smallTextFreqsAndCodes.txt" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/smallTextFreqsAndCodes.txt&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNGmI66iG9uQ_nR5gsspuG_jhgBJmg">smallTextsFreqsAndCod<wbr>es.txt</a> contains the expected frequencies and Huffman codes for this file.</span><span style="font-size: large;">Here is the complete small text file with 1s and 0s shown as chars, not stored as bits:</span>

    <ul>

     <li><span style="font-size: large;"><a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/Eyes_Count_Format_explicit.txt" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/Eyes_Count_Format_explicit.txt&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNEmxMMdqQ5YTtbKQjWPf33hEoOnfQ">using standard count format</a></span></li>

     <li><span style="font-size: large;"><a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/Eyes_Tree_Format_explicit.txt" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/Eyes_Tree_Format_explicit.txt&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNHZa99D82qdjxUHwIv9zTd76KjrNA">using standard tree format</a></span></li>

    </ul><span style="font-size: large;">You can use this <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/ExplicitBitOutputWriter.java" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/ExplicitBitOutputWriter.java&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNEmqQ7ybRWOqfMmpHB62SFdZmbL2g">ExplicitBitOutputWriter.<wbr>java</a> class to convert any file to a file with ASCII 0’s and 1’s. This is useful when looking at small files. You can compare files in Eclipse to find differences. <a href="https://stackoverflow.com/questions/4623564/how-do-i-compare-two-files-using-eclipse-is-there-any-option-provided-by-eclips" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://stackoverflow.com/questions/4623564/how-do-i-compare-two-files-using-eclipse-is-there-any-option-provided-by-eclips&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNGTrKqrabxk7U9fuDqo8DaYacbTkg">See this page for instructions.</a> Of course there are other programs that allow you to view the data in a file as raw 1’s and 0’s such as <a href="https://linux.die.net/man/1/xxd" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://linux.die.net/man/1/xxd&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNFPT1zXIFh21c7TD-Te1TY-v7pxPQ">xxd</a> on variations of Unix. </span><span style="font-size: large;">You may also find it useful to use a program that has the ability to view files as raw hexadecimal values. I use <a href="https://www.textpad.com/" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://www.textpad.com/&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNHE6QBF1RxGOkpCAQpB-Cab1X6FIQ">TextPad</a>but of course <a href="https://tinyurl.com/l6v9grq" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://tinyurl.com/l6v9grq&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNGLM246sOIj9eofYNrZOe9uQ7aqCw">there are many options</a>.</span><span style="font-size: large;"><b><code>Note: Expected return values for smallTxt.txt are:Standard Count Format:                Standard Tree Format:preprocessCompress returns -8138      preprocessCompress returns -120compress returns 8346                 compress returns 328</code></b></span></td>

   <td width="15%" height="19"><span style="font-size: large;">Provided by me</span></td>

  </tr>

  <tr>

   <td align="right" width="15%" height="15"><span style="font-size: large;">Large Test File</span></td>

   <td width="70%" height="15"><span style="font-size: large;"><a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/ciaFactBook2008.txt" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/ciaFactBook2008.txt&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNEww-Lock_85hJYxUFkOuMTnsljUw">The 2008 CIA Factbook</a>. The <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/ciaFactbook2008FreqsAndCodes.txt" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/ciaFactbook2008FreqsAndCodes.txt&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNHO3il1RasQmCOAzHwqDglLFPPgUA">ciaFactbook2008FreqsAndCod<wbr>es.txt </a>contains the expected frequencies and Huffman codes for this file, plus the standard tree for that file. <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/ciaFactBook2008.txt.hf" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/ciaFactBook2008.txt.hf&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNF-V9CvisfiSQ6ILt-csvwgjP2e5g">ciaFactbook2008.txt.hf </a>i<wbr>s the compressed file using the standard count format. <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/ciaFactBook2008_stf.txt.hf" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/ciaFactBook2008_stf.txt.hf&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNGsn7wlFT9Q0FhzP1MufkhZwD56LQ">ciaFactbook2008_stf.<wbr>txt.hf </a>is the compressed file using the standard tree format.</span><span style="font-size: large;"><b><code>Note: Expected return values for ciaFactbook2008.txt are:Standard Count Format:                Standard Tree Format:preprocessCompress returns 28867432   preprocessCompress returns 28874526compress returns 48230392             compress returns 48223298</code></b></span> <span style="font-size: large;">Explicit Bit Version of the header (no actual compressed data) <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/CIA2008_Factbook_SCF_Header_ExplicitBits.txt" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/CIA2008_Factbook_SCF_Header_ExplicitBits.txt&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNEXCr2Nl2Wj8MdDmt2twGA0j2rJag">Standard Count Format</a> (8256 bits)and <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/CIA2008_Factbook_STF_Header_ExplicitBits.txt" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/CIA2008_Factbook_STF_Header_ExplicitBits.txt&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNF-ou4g1rEl2tjFoSCe1GGiIU2FOw">Standard Tree Format</a> (1130 bits) for the CIA Factbook. These can be useful for debugging.</span></td>

   <td width="15%" height="15"><span style="font-size: large;">Provided by me</span></td>

  </tr>

  <tr>

   <td align="right" width="15%" height="15"><span style="font-size: large;">Large Test Files</span></td>

   <td width="70%" height="15"><p align="left"><span style="font-size: large;">Here are a couple of files to test your decompressor. I am not giving you the original file.<a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/mystery_count_header.bmp.hf" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/mystery_count_header.bmp.hf&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNHd468QMKuHDK7n8GOjAcNPRxhq0Q">mystery_count_header.bmp.hf</a>, <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/mystery2.bmp.hf" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/mystery2.bmp.hf&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNFfu1YnEGK3ZZUY8aBZCvD6A-8u5w">m<wbr>ystery2.bmp.hf</a> (uses count header), <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/mystery_tree_header.bmp.hf" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/mystery_tree_header.bmp.hf&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNElqtoeEu7cUmtjQ8N0kA6-LyTQ-w">mystery_tree_header.<wbr>bmp.hf</a></span></td>

   <td width="15%" height="15"><span style="font-size: large;">Provided by me</span></td>

  </tr>

  <tr>

   <td align="right" width="15%" height="15"><span style="font-size: large;">Test Framework and Files</span></td>

   <td width="70%" height="15"><span style="font-size: large;">To be sure your program is correct use this tester file: <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/A10_Huffman_Test_Student_Version.java" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/A10_Huffman_Test_Student_Version.java&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNFaZQIa08xQqFDlyZTB-8xvzPMOOg">A10_Huffman_Test_<wbr>Student_Version</a>. This is the same style test harness we will use when testing your submission, but we will use different files. Instead of using the HuffViewer with the GUI we use this implementation of IHuffViewer, a <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/DoNothingHuffViewer.java" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/DoNothingHuffViewer.java&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNHBcHG1umkqiwmeTpk5F7FJLbtl5A">DoNothingHuffViewer</a> when running the test harness. I recommend you create a separate package in your Eclipse project for these test files OR a whole different project from your working code.</span><span style="font-size: large;">To use the harness you need to download the <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/bevotest.jar" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/bevotest.jar&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNFaQPA7MrYmwLBt0ZxUgrpAUYKb8w">bevotest.jar</a> file created by <a href="https://www.cs.utexas.edu/~jthywiss/" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://www.cs.utexas.edu/~jthywiss/&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNGT8q1F2aUJyIccq9lGZE39Sq2bSw">John Thywissen </a>(former CS314 TA who wrote the testing framework we use to grade programs). bevotest.jar is a collection of code you need for the A10_Huffman_Test_Student_<wbr>Version to work. (The jar contains various .class files.) <a href="https://stackoverflow.com/questions/3280353/how-to-import-a-jar-in-eclipse" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=http://stackoverflow.com/questions/3280353/how-to-import-a-jar-in-eclipse&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNFH-ZkrtJ7b5oqGNXnRz41jRaYC2g">See this page for info on how to include a jar in your Eclipse project</a>.</span><span style="font-size: large;">Finally you need the <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/FilesForStudentTest.zip" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/FilesForStudentTest.zip&amp;source=gmail&amp;ust=1619291902554000&amp;usg=AFQjCNHHPHuSLxg7bvFPRg1PnwfgjNSGJA">test files in this zip file</a>. Download and unzip the file to your Eclipse project folder. </span></td>

   <td width="15%" height="15"><span style="font-size: large;">Provided by me</span></td>

  </tr>

  <tr>

   <td align="right" width="15%" height="15"><span style="font-size: large;">Files for Analysis</span></td>

   <td width="70%" height="15"><span style="font-size: large;"><a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/calgary.zip" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/calgary.zip&amp;source=gmail&amp;ust=1619291902555000&amp;usg=AFQjCNGio77UbeyLtzcVWrVQ080mWu7kCg">calgary.zip</a>, <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/waterloo.zip" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/waterloo.zip&amp;source=gmail&amp;ust=1619291902555000&amp;usg=AFQjCNH3TStuasgAeuz-WU_KnayrF0vb2w">waterloo.zip</a>, and <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/BooksAndHTML.zip" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/BooksAndHTML.zip&amp;source=gmail&amp;ust=1619291902555000&amp;usg=AFQjCNGMAW2kEtO6YHlAkbt8OHURKKSppg">BooksAndHTML.zip</a> zip files with lots of large files to test your finished program. Unzip the files and use the <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/doc/HuffMark.html" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/doc/HuffMark.html&amp;source=gmail&amp;ust=1619291902555000&amp;usg=AFQjCNHIKbpJsppehMET257Blu4O1gc39w">HuffMark</a> program / class to test your solution.</span></td>

   <td width="15%" height="15"><span style="font-size: large;">Links provided by me</span></td>

  </tr>

  <tr>

   <td align="right" width="15%" height="15"><span style="font-size: large;">Write Up</span></td>

   <td width="70%" height="15"><span style="font-size: large;">README.txt Write up will be an analysis of your experiments. What kinds of file lead to lots of compressions. What kind of files had little or no compression? What happens when you try and compress a huffman code file? </span></td>

   <td width="15%" height="15">Provided by you</td>

  </tr>

  <tr>

   <td align="right" width="15%" height="15">Yet More Test Files</td>

   <td width="70%" height="15"><a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/_SKYLER_huffman_files.zip" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/_SKYLER_huffman_files.zip&amp;source=gmail&amp;ust=1619291902555000&amp;usg=AFQjCNFbZptYOR8IdBRO-HI1uRAuLAHuWg">A zip with 6 more test files</a>, the compressed files in SCF and STF, and text results of counts and codes from a former student, Skyler.</td>

   <td width="15%" height="15"></td>

  </tr>

  <tr>

   <td align="right" width="15%" height="15">All Files</td>

   <td width="70%" height="15"><a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/A10_Huffman_All_Files.zip" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A10_Huffman/A10_Huffman_All_Files.zip&amp;source=gmail&amp;ust=1619291902555000&amp;usg=AFQjCNHaOE5CnDfazwZTIKFplfjV8Yah5w">All files except documentation in one zip. </a></td>

   <td width="15%" height="15">Provided by me</td>

  </tr>

  <tr>

   <td align="right" width="15%" height="19"><span style="font-size: large;">Submission</span></td>

   <td width="70%" height="19"><span style="font-size: large;">A10.zip with the following files: Your implementation of SimpleHuffProcessor, plus the classes you create on your own for the assignment. <strong>Do not turn in the provided classes. </strong>We will use them in their original form. (Meaning you cannot alter them or your program may not work when we test it.)</span></td>

   <td width="15%" height="19"><span style="font-size: large;">Provided by you</span></td>

  </tr>

 </tbody>

</table>

<b><span style="font-size: large;">Submission: </span></b><span style="font-size: large;">Add the <a href="https://www.cs.utexas.edu/~scottm/cs314/javacode/A6_Recursion/Recursive.java" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/javacode/A6_Recursion/Recursive.java&amp;source=gmail&amp;ust=1619291902555000&amp;usg=AFQjCNFl6BGKFDPnkkyCAys0wxrdhaXFNQ">standard header</a> to the SimpleHuffProcessor.java and copy it into the classes your create for the assignment.  Replace &lt;NAME1&gt; with your name and &lt;NAME2&gt; with your partner’s name if working with a partner. Note, you are stating, <u>on your honor</u>, that you did the assignment on your own or with your partner.</span>

<span style="font-size: large;">Create a zip file name a10.zip with your SimpleHuffProcessor.java, <b>the .java files for the other classes your create</b>, and you README.txt. The zip file must <b>not</b> contain any directory structure, just the required files.</span>

<a href="https://www.cs.utexas.edu/~scottm/cs314/handouts/creating_a_zip_file_via_eclipse.htm" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://www.cs.utexas.edu/~scottm/cs314/handouts/creating_a_zip_file_via_eclipse.htm&amp;source=gmail&amp;ust=1619291902555000&amp;usg=AFQjCNEwNOyTKzFmW4TfPxSJTbDbN9oKSw"><span style="font-size: large;">See this page for instructions on how to create a zip via Eclipse. </span></a>

<p align="left"><span style="font-size: large;">Turn in a10.zip <a href="https://guides.instructure.com/m/4212/l/41972-how-do-i-submit-an-online-assignment" target="_blank" rel="nofollow noopener" data-saferedirecturl="https://www.google.com/url?q=https://guides.instructure.com/m/4212/l/41972-how-do-i-submit-an-online-assignment&amp;source=gmail&amp;ust=1619291902555000&amp;usg=AFQjCNHtGp1oS1DmL5c6l20TcG_5FQljjA">via your Canvas account</a> to programming assignment 10. </span>

<ul>

 <li><p align="left"><span style="font-size: large;">Ensure you files are named correctly. Failure to do so will result in points off. Ensure any other files you create do not conflict with the given Java classes.</span></li>

 <li><p align="left"><span style="font-size: large;">Ensure SimpleHuffProcessor.java.and other classes are part of the default package. Do not add a <code>package</code> statement to any of your files.</span></li>

 <li><p align="left"><span style="font-size: large;">Ensure your zip has no internal directory structure. When the file is unzipped no directories (folders) are created. (Note, the built in unzip feature of some versions of Windows and Apple OS X “help” by adding a directory when you unzip with the same name as the file. The unzip we use on the CS Linux system does not do this. Neither do unzip programs such as 7zip.)</span></li>

 <li><p align="left"><span style="font-size: large;">Ensure you submit the assignment under Programming Assignment 10 in Canvas.</span></li>

 <li><p dir="ltr" align="left"><span style="font-size: large;">We will compile and run our tester harness on the CS department Linux machines. To ensure you have no problems (strange imports, package statements) I suggest you move your files to a folder on your CS department account and compile and run them from the command line.</span></li>

</ul>