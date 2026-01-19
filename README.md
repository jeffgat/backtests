# orb_backtests

### HUGE ISSUES
- identfying gaps correctly but we are entering them as they're created instead of on the retest. must address this

- running into these "adverse executions" that are causing me to lose more than 1R per position. sometimes this is 2-4R, and in really bad cases it can be like 9-18R lost on a single trade. seems to be an issue with stops not executing correctly and eod flattens or positions being held overnight.

- while the above is messing with the long term data, 1-2 years back seems to be okay? but it's still going to be inaccurate because my max wins are also 1.1R  - 1.2R when it should be 1.5R.

- so we need to figure out how to get more precise executions bc we don't really run into slippage or spreads this bad.