# Deuterium layout

## Main layer
![](./assets/main.png)

## Symbol+Nav layer
![](./assets/layer.png)

## Cyanophage layout analyzer
![](./assets/cyanophage-2.png)
 
[link (select "angle mod")](https://cyanophage.github.io/playground.html?lan=english&layout=%5Cou.%27xfrlbzeaicpmdntsv%2F%2Cwgyhkjq%3B-%5Eback&mode=iso&thumb=l)

## Benefits
- High efficiency due to very low SFBS, SFS (and redirect SFS). It should feel quite fluid as all fingers are equally utilized
- `y` can be typed with either hand, depending on letter sequence. `y` interacts with nearly all english letters and this eliminates a lot of same finger bigram/skipgram problems
- Sufficient alternation between hands and between (adjacent) fingers (**it is quite hard to achieve this**)
- Having many letters on the homerow
- High inrolls/outrolls ratio (outrolls can feel less natural if they are on the pinky/ring)
- Having hjkl on the same hand in a relatively natural positions (vim + tiling window managers)
- Very low 2u sfs
- Bottom row on the ring/pinky is kept very light which helps with scissors (My older versions didn't do so well here)

## Design choices (some of it can be controversial)

#### Pushes frequent letters to the outer ring/pinky
This allows the index fingers to move inward and reach inner column letters such as `y`, `p` and `x` more easily. In technical term, this reduces overall Lateral Stretch Bigrams (LSBs)

#### `E` being on the pinky position
I have `e` on pinky finger for almost a year, it is not really a problem for me personally. I suspect that it may be a problem if `e` were to be on the right hand, as the right pinky has the additional burden of hitting BACKSPACE, ENTER, and punctuations (hence very easy to injure yourself when first starting out and correcting a lot)

#### Having `H` at the qwerty `N` position
H is somewhat frequent in common english, but there are several reasons I placed it there :
- it eliminates 2u (2 rows) jump on the index fingers
- it allows `why` to be typed in this sequence: Left index -> right index -> right index
- it prevents index finger from being curled up in the `k` (qwerty `m`) position, which makes `y`/`x` harder to reach

#### Right pinky having extra letters `Z` and `V`
The `v` position may a dealbreaker for some, but they are not unreasonable because `v` is usually a skipgram with another consonants (exceptions being `r`, `n`, `l`). And most of the letters that interact heavily with `v` are assigned to index finger, so there's sufficient runway. `z` is in the most awkward position but it is the least frequent letter in english. 

```
SHAI
vr + rv: 0.06%
  vr: 0.00%
  rv: 0.06%
vl + lv: 0.03%
  vl: 0.00%
  lv: 0.03%
vn + nv: 0.05%
  vn: 0.00%
  nv: 0.05%
Total: 0.14%
```

```
SHAI
v_l + l_v: 0.25%
  v_l: 0.15%
  l_v: 0.10%
v_t + t_v: 0.16%
  v_t: 0.05%
  t_v: 0.11%
Total: 0.41%
```

## Cmini

``` 
deuterium
  _ o u . '  x f r l b z
   e a i c p  m d n t s v
    / , w g ȳ  h k j q ;  

SHAI:
  Alt: 33.10%
  Rol: 40.77%   (In/Out: 23.24% | 17.53%)
  One:  1.00%   (In/Out:  0.58% |  0.41%)
  Rtl: 41.77%   (In/Out: 23.82% | 17.94%)
  Red:  3.01%   (Bad:     0.15%)

  SFB:  0.76%
  SFS:  4.49%   (Red/Alt: 0.72% | 3.78%)

  LH/RH: 49.85% | 50.15%
```

## Fingermap

from left pinky (0) to right pinky (7)
```
  _ o u . '  x f r l b z
   e a i c p  m d n t s v
    / , w g ȳ  h k j q ;  

  0 1 2 2 3  4 4 5 6 7 7
   0 1 2 3 3  4 4 5 6 7 7
    1 2 3 3 3  4 4 5 6 7  
```

# Resources (from AKL discord server)
- Keyboard Layouts Doc - A very thorough document with in-depth explanations of typing and layout theory | https://docs.google.com/document/d/1W0jhfqJI2ueJ2FNseR4YAFpNfsUM-_FlREHbpNGmC2o
- Dreymar's Big Bag - A collection of modifications and other useful tricks | https://dreymar.colemak.org/
- gfruit's Words Filter - A simple yet incredibly useful tool for finding words with certain bigrams, characters, and fingers | https://gfruit.github.io/typing/words-filter.html
- Octa's Keymap Creator- A tool for creating and sharing layout fingermaps | https://keymap-creator--octatypes.repl.co/ 
- Monkeytype Fingermap - Same as above, made by the creator of MonkeyType | https://fingermap.monkeytype.com/
- MSKLC Guide - Documentation for the Windows layout creator tool | https://msklc-guide.github.io/#2
- Guide to alt layouts - A helpful introduction to alt layouts | https://getreuer.info/posts/keyboards/alt-layouts/
- Keyboard Layout Tryout - tool for testing how layouts feel by converting text | https://keyboard-layout-try-out.pages.dev/
