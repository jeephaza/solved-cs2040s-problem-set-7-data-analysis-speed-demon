Download Link: https://assignmentchef.com/product/solved-cs2040s-problem-set-7-data-analysis-speed-demon
<br>
We live in a world overwhelmed with information. Every two days, we create as much new information as was created in the entire history of human civilization up until 2003 (according to Eric Schmidt, the CEO of Google). We produce more than 3 exabytes of data per day! Much of this data is stored in large databases, and one of the challenges today is to rapidly process and analyze all the data. Since the databases are so large, it requires very fast algorithms and data structures that are highly optimized for maximum efficiency. In this competition, you will try to develop the <em>fastest </em>algorithm for analyzing a large dataset.

When analyzing a large dataset, there are many different goals. We will focus on a particular type of data mining in which we want to discover properties and patterns of the underlying data. Frequently, we want to know various statistics: the average, the median and the mode. Often, we also want to know about patterns: how often do users of a certain profile (e.g., males between the ages of 18 and 32) buy a certain item? Often, we want to know about correlations: how often does a user who buys item <em>A </em>click on link <em>B</em>?

For the purpose of this competition, we define an abstract data mining problem that involves finding correlations in our data set. The database consists of a large set of very large data entries. The goal is to find how many pairs of entries are identical, i.e., contain the same information. Your job is to implement a data mining program that reads in the database and performs this analysis <em>as fast as possible</em>.

<h1>Problem Details</h1>

We now describe the details of the competition more precisely.

<strong>Input. </strong>The input “database” is a file consisting of a set of lines of text, each of which represents one entry. Each line of text contains a large number of characters. (Notice that the lines may consist of thousands, or even tens of thousands, of characters.)

Your program will implement a single public method: public int processData(String filename). This method will take a filename as an input. It should then parse the file and process the data in the file. Finally, it should return an integer as the answer. (We have given you an existing class file template to use.)

The format of the input is as follows. The first line of the database contains a single integer <em>i</em>, which represents the number of entries in the database. It is followed by <em>i </em>lines, each containing an arbitrary number of characters and ended by an end-of-line character (ASCII character 10). Note that entries may consist of any of the 128 legal ASCII characters, except for 10 and 13 (which indicate a new line). Characters may be repeated, and entries may be of any length.

<strong>Output. </strong>Your program should calculate the number of pairs of entries that contain an identical multiset (i.e. multiple instances of the same character are allowed) of characters. Notice that the characters may appear in any order: two entries <em>e</em><sub>1 </sub>and <em>e</em><sub>2 </sub>are equivalent if <em>e</em><sub>1 </sub>is equal to some permutation of <em>e</em><sub>2</sub>. You should print your output, which should consist of an integer, followed by a newline character.

<strong>Example.         </strong>The following is an example of an input database:

7

BCDEFGH

ABACD

BDCEF

BDCAA

DBACA

DABACA

DABAC

The appropriate output in this case is:

6

In particular, note the following six pairs of equivalent entries:

(ABACD, BDCAA)

(ABACD, DBACA)

(ABACD, DABAC)

(BDCAA, DBACA)

(BDCAA, DABAC)

(DBACA, DABAC)

<h1>Rules</h1>

The following are the rules of the competition:

<ul>

 <li>Your solution must be written in Java.</li>

 <li>You may use any available Java libraries. (I should note that I do not expect the fastest solutions to rely heavily on existing libraries.)</li>

 <li>You are allowed to submit only one final program.</li>

 <li>All programs must be written entirely by you. You may use any ideas or algorithms that you find on the internet, in books, etc. However, all the submitted code must be written by you. • The competition will end on Friday, April 3 at 11:59pm.</li>

 <li>You may continue to update your solution up until the deadline. The final winner will be determined by testing that occurs after the competition ends.</li>

</ul>