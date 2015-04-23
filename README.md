# SpecialKEval

SpecialKEval is a lightweight 32-bit Texas Hold'em 5- and 7-card hand evaluator 
written in C++.

0 = Ace of Spades
1 = Ace of Hearts
2 = Ace of Diamonds
3 = Ace of Clubs

4 = King of Spades
5 = King of Hearts
6 = King of Diamonds
7 = King of Clubs
...

## Example

```
#include <iostream>
#include "SevenEval.h"

int main() {
  SevenEval const* eval = new SevenEval();
  // Get the rank of the seven-card spade flush, ace high.
  std::cout << eval->GetRank(0, 4, 8, 12, 16, 20, 24) << std::endl;
  delete eval;
  return 0;
}
```
