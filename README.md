# tortoise-and-hare
Tortoise and hare are racing in ram!


The animals begin at "Square 1" of 70 squares. Each of the squares represents a position the animal can hold along the racetrack. The finish line is at Square 70. When an animal wins, a winning message posted. For example:

Yay! The rabbit won! He hops the fastest!

Woo-hooo! Slow and steady wins the race! Congratulations, turtle!

Tie score--no winner! Want to race again?

To start the race, print a message similar to:

Bang! Off they go!

There is a clock that ticks once per second. With each tick of the clock, the program should adjust the position of the animals according to the following rules:

|Animal  | Move Type | Percentage of the Time | Actual Move|
---------|-----------|------------------------|-------------|
Tortoise | Fast Plod | 50%                    | 3 squares to the right|
Tortoise | Slip      | 20%                    | 6 squares to the left |
Tortoise | Slow Plod | 30%                    | 1 squares to the right|
Hare     | Sleep     | 20%                    | No move at all |
Hare     | Big Hop   | 20%                    | 9 squares to the right|
Hare     | Big Slip  | 10%                    | 12 squares to the left|
Hare     |Small Hop  | 30%                     |1 square to the right|
Hare     |Small Slip | 20%                     |2 squares to the left|

If an animal slips, the lowest it can go is back to position 1. The highest it can go is to position 70 when it wins the race.

The percentages in the table above were used and a random integer called 'current' was generated randomly within the range of 1 to 10.

For the tortoise, a "fast plod" is when 1≤ current ≤ 5, a "slip" when 6 ≤ current ≤ 7, or a "slow plod" 8 ≤ current ≤ 10. A similar approach would be used to set up the moves for the hare.

For each tick of the clock (each repetition of the loop), print a 70-position line showing the letter T in the tortoise’s position and the letter H in the hare’s position. If the two animals land on the same square, which may happen, the animals will bump. If this happens, print BUMP! at the current position.

After each line is printed, it is checked whether the tortoise and the hare are on Square 70. If this is the case, a message of the winning type is printed.

It may make the simulation more interesting if you have users press any key after each iteration of the loop, so that they can see the movement of the animals.


