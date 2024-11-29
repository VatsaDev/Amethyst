# Language Design

## pythonian features

 - easy input
 - good STL
 - easy syntax

Pretty easy, heres some examples:

Easy input:

Pretty much any ICPC problem, CF, AoC, etc, can all have their inputs entered in 5-10 lines of python, and I really like that

Example from Guard Evaders (ncna24, problem F)

```
4 1
RFRL
```

```python
l1 = input().split(" ")
g = int(l1[0])
p = int(l1[1])
l2 = input()
print(g,p,l2)
```

Good STL:

I like "I can import anything" part of python, and I will most likely implement small parts of the python standard library overtime, but I would like enough to be able to complete AoC with it, so by order of priority

 - `import math` going to be big
 - fileio, need minimum ability to read files
 - probably need some sort of counter/hashmap thing
 - some equivalent of itertools permutations/combinations
 - regex/strings(.sort, .reverse, slice, etc) type lib
 - probably part of the language itself, but lots of DSA stuff, ex. dp, linked lists, trees/graphs, DFS/BFS, etc

Other stuff I'll probably add to the STL for more general use:

 - types, beyond just the usual int8/fp16/char, etc, maybe actually implement types that can be user defined, ex [alcuin](https://x.com/scheminglunatic), who recommended types like `direction = up|down|left|right`
 - some try catch with default exceptions
 - datetime, csv, hashlib, gzip, os, io, threading&multiprocessing, etc
 - asyncio, urllib, tkinter equiv

Easy syntax:

Fairly obvious, cpp is nice, but still a big believer of less brackets and stuff

```cpp

#include <bits/stdc++.h>

using namespace std;

int main() {
  cout << "Hello World!" << "\n";
}

```

```py
print("Hello World!")
```


## haskellian features

 - being really functional

I mostly like how the purely functional setup looks, also one liners

ex. one liner for watermelon (beginner CF)

```
main :: IO ()
main = getLine >>= putStrLn . (\w -> if w > 2 && even w then "YES" else "NO") . read
```

## amethyst pseudocode

## other cool stuff I might add overtime

 - a proper module system, so people can actually make third party libs for the lang
 - amethysts equivalent for pytorch, probs simpler, basicML lib
 - networking stuff, tcp/udp, ports, etc
 - sveltekit type lib, or django equiv
 - matplotlib, but with a more wandb style soft theme by default
 - not part of the lang, but llama amethyst would be funny
