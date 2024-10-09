# CI2024_lab1

In this laboratory we are going to use different algorithms to resolve the set cover problem. I implemented the Greedy and the Hill Climbing algorithms. Hill Climbing is developed in two different ways, one using a single tweak mutation and one using a multiple tweak mutation. In particular, with the single-tweak we are going to mutate one single element of the solution, on the other hand, with the multi-tweak we are going to mutate multiple elements of the solution.

## Results

#### Greedy algorithm

| UNIVERSE_SIZE | NUM_SETS | DENSITY | COST |
| :- | :- | :- | :- | 
| 100 | 10 | .2 | 283.98
| 1_000 | 100 | .2 | 6_159.13
| 10_000 | 1_000 | .2 | 99_252.33
| 100_000 | 10_000 | .1 | 1_512_712.07
| 100_000 | 10_000 | .2 | 1_727_021.90
| 100_000 | 10_000 | .3 | 1_769_696.74

#### Hill Climbing with single tweak

| UNIVERSE_SIZE | NUM_SETS | DENSITY | NUM_ITERS | COST |
| :- | :- | :- | :- | :- |
| 100 | 10 | .2 | 100 | 283.98
| 1_000 | 100 | .2 | 100 | 13_396.14
| 10_000 | 1_000 | .2 | 100 | 1_996_722.33
| 100_000 | 10_000 | .1 | 100 | 122_474_731.31
| 100_000 | 10_000 | .2 | 100 | 260_788_280.14
| 100_000 | 10_000 | .3 | 100 | 409_589_136.23

#### Hill Climbing with multiple tweak

| UNIVERSE_SIZE | NUM_SETS | DENSITY | NUM_ITERS | COST |
| :- | :- | :- | :- | :- |
| 100 | 10 | .2 | 100 | 283.98
| 1_000 | 100 | .2 | 100 | 13_075.15
| 10_000 | 1_000 | .2 | 100 | 1_991_860.34
| 100_000 | 10_000 | .1 | 100 | 122_806_230.17
| 100_000 | 10_000 | .2 | 100 | 264_756_379.83
| 100_000 | 10_000 | .3 | 100 | 410_068_612.21

We can conclude that the Greedy algorithm achieves better results in comparison with Hill Climbing. That's because the greedy algorithm for each iteration takes the set that covers the greatest number of elements; otherwise, Hill Climbing for each iteration explores numerous nearby solutions, by doing this, it can get stuck in a local optimum.

Finding a great way to develop the greedy algorithm I discuss with @YounessB1.