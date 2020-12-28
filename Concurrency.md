# Concurrent & Parellel programming

## Difference between concurrency and parellelism

I looked up many articles online about the difference between these two concepts. Some of them are explaining pretty well while others are not. However, nearly all of them couldn't explain one question, `concurrent` and `parellel` are synonyms in English dictionaries, both interpreted as happening 'at the same time' but why they have so different meanings, especially when `concurrent` is also related to time slicing. 

I believe every terminology/concept is a noun. A noun is supposed to have its etymology. In my past experience, the etymology of a word helped me a lot in explaining the concept that I don't understand first. Therefore, I looked up dictionaries more carefully. However, the Latin etymology didn't help much. The mostly used meanings of `concurrent` still confused me. Meanings from Merriam-Webster: operating or occurring at the same time; running parallel,  from Oxford English Dictionary: Runing together in space, as parellel lines.  

I also found its (`concurrent`) meaning in mathematics, which is (of three or more lines) meeting at or tending towards one point, based on Concise Oxford English Dictionary. It doesn't help much as the etymology, but providing some hints for me. Then I looked through this in mathematical fields. Sadly, little progress was made.  

How about searching for `concurrency`? I ever searched the word in the dictionary. But it didn't have much meanings as `concurrent` and I thought `concurrent` is the root for `concurrency` and didn't even look it through. However, I tried to look through it one more time to see if further progress could be made. Then I found something exciting in Oxford English Dictionary, which is a running together in place or time. Notice that, unlike `concurrent`, there is no 'parallel lines' explanation appended. 

Until now, though it provides some clues of the question, I still can't connect the dots to answer it. Then I look through wikipedia (of course I skimmed it like the case of `concurrency` in OED, but didn't read it through). I then found some really exciting results in the `history` entry of `Concurrent computing`. Here is word to word copy from Wikipedia:

> Concurrent computing developed out of earlier work on railroads and [telegraphy](https://en.wikipedia.org/wiki/Telegraphy), from the 19th and early 20th century ... These arose to address the question of how to handle multiple trains on the same railroad system (avoiding collisions and maximizing efficiency) ... The academic study of concurrent algorithms started in the 1960s, with [Dijkstra (1965)](https://en.wikipedia.org/wiki/Concurrent_computing#CITEREFDijkstra1965) credited with being the first paper in this field, identifying and solving [mutual exclusion](https://en.wikipedia.org/wiki/Mutual_exclusion).

Then I looked through other entries of concurrent in Wikipedia, especially the meanings in roads system, which is the etymology I mentioned in the beginning.   Then I found the answer. Here is word to word copy from `Concurrency (road)` in Wikipedia:

> A **concurrency** in a road network is an instance of one physical roadway bearing two or more different [route numbers](https://en.wikipedia.org/wiki/Route_number).

This concept suddenly coincides with the hints from the English dictionaries. If we virtualize road as critical section, then it becomes the core of `mutual exclusion` in academic paper by [Dijkstra (1965)](https://en.wikipedia.org/wiki/Concurrent_computing#CITEREFDijkstra1965). If we virtualize road as certain time period of a single core, then it becomes the core in many online explanations about difference between `concurrency` and `parellelism`, because like one physical road can only bear one route number at a specific time , a single core can only execute one execution step of one process (may not be accurate description, but approximate). 

I think this will be the most direct way of explaning the difference between these two concepts, in a road perspective. 





