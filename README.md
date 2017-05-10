# Spell checker using BK trees

We have used BK trees instead of suffix trees / ternary tree / trie trees to correct a word.

Proposed by Burkhard and Keller in 1973, the BK-Tree is a data structure used for spell checking based on the Levenshtein Distance between two words, which is basically the number of changes you need to make to a word to turn it into another word. 

Some example distances:

* LevenshteinDistance(cook, book) -> 1
* LevenshteinDistance(cook, books) -> 2
* LevenshteinDistance(what, water) -> 3

## About the project
Spelling verification and correction had been at the core of many technologies in the past decade, which saw a rise of search engine giants. Features of spell correction and suggestion made searching for terms quite easy for the users. Millions of users across the world use such search engines, hence implementation of such features need highly efficient algorithms as well. Traditionally trie trees have been used to achieve those features, which are highly time efficient, but space efficiency has always been a constraint for the data structure. Here, without affecting the time efficiency, this approach has the potential to improve the space efficiency.<br>

BK trees are formed based on discrete distance between two variables. For finding a discrete distance between two words, Levenshtein distance(also known as edit distance) seems appropriate as it provides us an efficient opportunity to correct the word as well. Levenshtein distance is nothing but the number of characters different between two words. For eg : the  LD between cat and bat is ‘1’ since only one character is different between them. Another way of defining levenshtein distance is : the number of changes required to transform a word into another word is the LV between them. <br>

Using BK-trees and Levenshtein distance, the aim is to return bat or cat when we enter gat (where ‘gat’ is not a word in the dictionary). What makes BK trees so special is that it takes a problem which has no obvious solution besides brute force method and provides us with a simple and elegant solution. <br>

## Note: This code can only be exexuted in windows.
