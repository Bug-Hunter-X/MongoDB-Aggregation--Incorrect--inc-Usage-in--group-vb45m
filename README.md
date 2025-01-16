# MongoDB Aggregation: Incorrect $inc Usage in $group

This repository demonstrates a common error when using the `$inc` operator within the `$group` stage of a MongoDB aggregation pipeline.  The `$inc` operator is intended to increment a numeric field, but its use within `$group` requires careful consideration.

The incorrect usage shown in `bug.js` leads to unexpected results. The correct usage is demonstrated in `bugSolution.js`.  The `$sum` operator should be used to accumulate values within the grouping stage.

## How to reproduce

1.  Clone this repository.
2.  Ensure you have MongoDB running and configured.
3.  Run `bug.js` to see the incorrect behavior.
4.  Run `bugSolution.js` to see the corrected behavior.