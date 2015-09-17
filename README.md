# Sequential-PageRank


SequentialPageRank is a java file that calculates the page ranks of different “sites” that link to other “sites” which are provided in an input file, the top 10 "sites" with their page ranks are printed to the console while all sorted "sites" and their page ranks are written to an output text file like the one provided in this repo. The format for the input files looks as such:

`0 \n
1 2
2 1
3 0 1
4 1 3 5
5 1 4
6 1 4
7 1 4
8 1 4
9 4
10 4`

In reality they aren't websites, they are just integers. This was a good exercise to test out the pagerank algorithm itself, before moving onto websites.


In a terminal, while in the same directory as where the java file lives, to run the program it first needs to be compiled using: javac -g SequentialPageRank.java. This will generate two class files, one will be of the same name as the java file and the other is a custom class called Tuple written to help sort the end result.

The program is then ran using the following format: java SequentialPageRank <input file path> <output file path> <number of iterations> <dampening factor>. The file paths for input and output should be the absolute paths and in quotations.


When running the file I usually used 10-1000 iterations, with a dampening factor of .85.


Something like this should be printed to the console:

These are the top 10 pageranks:

[1: 0.38440094881355447]

[2: 0.34291028550838]

[4: 0.08088569323449772]

[3: 0.03908709209996609]

[5: 0.03908709209996609]

[0: 0.03278149315934399]

[6: 0.016169479016858404]

[7: 0.016169479016858404]

[8: 0.016169479016858404]

[9: 0.016169479016858404]

[10: 0.016169479016858404]