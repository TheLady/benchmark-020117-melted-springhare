### 15: Finite State Gate

You just installed a new remote controlled gate, and you're having a blast playing with the remote clicker.

The clicker works like this:

If the gate is `OPEN` or `CLOSED`, clicking the remote will cause the it to move, until it completes the cycle of opening or closing.

```Gate: Closed -> remote clicked -> Gate: Opening -> Cycle complete -> Gate: Open.```

If the gate is currently opening or closing, clicking the remote will make it stop where it is.

When clicked again, the gate will go in the opposite direction, until the cycle is complete or the remote is clicked again.

The gate starts `CLOSED`.

**Example Input:**

```
remoteClicked
cycleComplete
remoteClicked
remoteClicked
remoteClicked
remoteClicked
remoteClicked
cycleComplete
```
**Example Output:**

```
Gate: CLOSED
Remote clicked.

Gate: OPENING
Cycle complete.

Gate: OPEN
Remote clicked.
Gate: CLOSING

Remote clicked.
Gate: STOPPED_WHILE_CLOSING
Remote clicked.
Gate: OPENING
Remote clicked.
Gate: STOPPED_WHILE_OPENING
Remote clicked.
Gate: CLOSING
Cycle complete.
Gate: CLOSED
```
### Strategy
gate open - can move right, how far?
gate closed - can move left
gate opening - current position
gate closing - current position
  how do you keep gate from crushing the kid (or whatever),
  if gate is moving in one direction, button push makes it stop 
  next button push switches direction
  next button push switches direction

start by settiong positions to false  

switch statements and prototypes
https://teamtreehouse.com/library/programming-stepbystep-objectoriented-javascript-part-1






