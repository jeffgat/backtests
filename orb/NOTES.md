# NOT YET, BUT SHOULD BE IMPLEMENTED. CHANGES TO PROD
- implement ATR
- size gaps in NY as 1.75% of the ATR
- size gaps in asia as 0.25% of the ATR

## ideas
- can we use ATR to create dynamic stops that scale with price? or is the 2 candle stop the best?
- can we use ATR to optimize the gap size for which we enter on? - yes
- can we use ATR to optimize tp targets?
- only enter if a nearby 5m gap has been "respected"
- multiple orbs
  - 2 a day?
  - one more attempt only if first one failed?

### ATR, feb 5 2026
- for orb as a continuation model, we see most of the winning orbs occur when price is past 100% of its ATR
- this means that price is expanding
- we should never look at how far past TP is relative to ATR -- this kills your R
- we want to take ORBs in environments where price is blasting well past ATR

### ATR, feb 6 2026
- validating gaps by requiring a minimum % of daily ATR (14) allows the entry to be more robust in different price environments
- increased R in both asia and NY on NQ
- potential for this to be used on ES as well, needs further testing
- GC during the bear market shows a smooth NEGATIVE equity curve
  - can this be used to create a reversal model? targeting back inside the OR after a breakout?
  - what other assets can we use this on?
  