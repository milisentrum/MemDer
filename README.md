# Work Space
### Content
</p>
*  <a href="#Algorithm Rutishauser">Algorithm Rutishauser</a> 
*  <a href="#Binary search">Binary search</a> 
*  <a href="#Crossword">Crossword</a> 
*  <a href="#Directory depth">Directory depth</a> 
*  <a href="#FindSimilar">FindSimilar</a> 
*  <a href="#Generic Collections">Generic Collections</a> 
*  <a href="#HashSearchFile">HashSearchFile</a> 
*  <a href="#Largest path">Largest path</a> 
*  <a href="#Sort by length">Sort by length</a> 
*  <a href="#Tower of Hanoi">Tower of Hanoi</a> 
*  <a href="#Word generator">Word generator</a> 
</p>

# [Algorithm Rutishauser](https://github.com/Feodoros/WorkSpace/blob/master/AlgorithmRutishauser/StructureList.cs)

Feature: full bracket structure of the expression. Example:
D:=((C-(B*L))+K)

The algorithm assigns each character from the string a level number

1. If it is an opening bracket or a variable, then the value is increased by 1;

2. If the operation mark or closing bracket, then decreases by 1.

The algorithm consists of the following steps:

1. complete the leveling;

2. search for line items with the maximum level value;

3. select three - two operands with the maximum value of the level and the operation that is concluded between them;

4. The result of computing the triples is denoted by an auxiliary variable;

5. remove the selected triple from the source line along with its brackets, and put in its place an auxiliary variable indicating the result, with the level value one less than the selected triple;

6. Perform items 2 - 5 until one variable remains in the input line, indicating the general result of the expression.

In addition, we implemented our list based on an array. It has: indices, count, add (in any place), remove, etc.

# [Binary search](https://github.com/Feodoros/WorkSpace/blob/master/BinSearch/Program.cs)
![](https://sun9-15.userapi.com/c857320/v857320109/180096/002vsj8buk8.jpg)
Search the coordinates of an element in 2d array.

We have a sorted array from smallest to largest. We find the middle of the line of the array and compare the element arr [i, mid] with X ( i - number of line in the array). If they match, the problem is solved. if not, then we increase or decrease the right and left borders depending on whether our element is smaller or greater than X.

# [Crossword](https://github.com/Feodoros/WorkSpace/blob/master/Cross/Program.cs)
You have a key word and an array of words (their number is equal to the number of letters in the main word). The algorithm outputs an array with the key highlighted by the word.
We are looking for the intersection indices of words with the word key
Pad each word with spaces
And display
![](https://sun9-58.userapi.com/c205828/v205828109/10aea6/f3boQI59Slc.jpg)


# [Tower of Hanoi](https://github.com/Feodoros/WorkSpace/blob/master/HanoiTowards/Program.cs)
![](https://blog-c7ff.kxcdn.com/blog/wp-content/uploads/2016/12/Tower-of-hanoi.gif)

## About algoritm
We have 3 pegs.
Task: transfer discs from one peg to another using the third peg.


We recursively solve the Hanoi tower problem for n rings.
If the towers n = 3, then we solve the problem for n = 2, and then for n = 1 (with each decrease in n, our maximum ring decreases, that is, recursively going down, we climb the tower).
The case n = 1 is the recursion stopping point.

<p align="center">
  <a>
      <img src="https://user-images.githubusercontent.com/32129186/55137420-f9f7c700-5141-11e9-997f-31a76a4693a7.gif" alt="MemDer" width="200"></a>
  </a>  
</p>

## Key Features
  
* Smart feed will adjust depending on user meme preferences
* Content is aggregated from differenet groups 
  - each day new most liked memes are added to database
* User is able to communicate with other users
  - app sorts users by similarity with your preferences
* Swipes mechanics allows user to assess seen memes 
  - super dislike - dislike - like - super like
<pre>
<p align="center">
  <a>
    <img src="https://user-images.githubusercontent.com/32129186/55136074-7688a680-513e-11e9-884f-e2737bd4ab37.gif" width="300">
  </a>
</p>
</pre>

## Description

Nowadays you won't surprise somebody with an app that allows you to find people with similar interests. 

In MemDer communication forms on humor preferences because humor is a thing that connect people.
You are able to see and assess memes - smart feed will show memes that specifically you are interested in. 
Your meme preferences will define who you are going to communicate with. 
It is great when you always have people with whom you can laugh!
But if you just want to see some funny pictures from different groups - just open MemDer once!

## Download

You can [download](https://play.google.com/store/apps/details?id=com.MemDerPack) the latest version of MemDer on Google Play.

## Credits

MemDer uses the following open source packages:

- [VK parser](https://github.com/Feodoros/vkParser)
- [Firebase](https://firebase.google.com)
- [Azure](https://azure.microsoft.com/ru-ru/)
- [fabric](https://get.fabric.io)
- [CardStackView](https://github.com/yuyakaido/CardStackView)

## Creators

- [Zhilkin Fedor](https://github.com/Feodoros)
- [Smirnov Alexander](https://github.com/SmirnovAlexander)
- [Galochkin Alexander](https://github.com/alexandr-galochkin)

## Creating history

It all began on VK hackathon. We were given a case where we should have done an app with entertaining content.
After a long time thinking and discussing we came up with an idea: "Why don't we make something new in domain of humor and dating?".
Sounds weird. But we believed in this and started to develop the idea. So we made what we made! 
Firstly we called it "Laugh and Love", but nobody liked the name. In the mean time we gave name "MemDer" to the folder with project.
So, as it usually happens, everybody enjoyed it: laconically and telling.
This is how appeared a reason to work many days at our project.
So MemDer was born!
