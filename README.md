# Backshotter
Buckshot Roulette Bot using Alpha-Beta Pruning.

First goals:
- need a way of entering in the state of the game, because image recognition ain't gonna work
  well for the dealer's items.
- Create evaluation for end of a set (no shots left) based on heath and items.
- Plan is to keep track of all possible orderings rather than using chance.
  - will cause more branching, but should make keeping track of future shells (from burner phone) easier
  - should probably make use of storing evaluations like a Transposition table in chess,
    since we can arrive at the same scenario in different ways.
  - store as tree structure? When a shot is fired, 
    go down the associated branch (blank is left, live is right)?
- weight evaluations based on their likelihood. Each scenario is equally weighted
