# UTSA_GPS_DATA
This GPS dataset has been recorded on UTSA campus parking lot on June, 1, 2017.

Clean Data:

-SateState is a cell array. SatState{k} renders the following information for the visible satellites at epoch k:
 
 data:           [Sat ID , pseudorange (m) , Pseudorange rate (m/s), Sat Position (m) in ECEF, Sat clock bias, Sat Velocity (m/s) in ECEF, Sat clock drift]
 column index:       1           2                   3                           4:6                 7                      8:10                  11


-xState is a matrix. xState[k] renders the following information at the receiver at epoch k:

 data:            [ xCoordinate (m)    yCoordinate (m)    zCoordinate (m)    ClockBias (m)    xVelocity (m/s)    yVelocity (m/s)     zVelocity (m/s)    ClockDrift (m/s)]
 column index:             1                  2                 3                 4                 5                    6                 7                8

* The clock bias and clock drift are the estimates obtained from the solutions of Weighted Least Squares (WLS).
-WP is the diagonal uncertainty in pseudorange.  WP{k} renders the uncertainty in pseudoranges for the visible satellites at epoch k.
-WR is the diagonal uncertainty in pseudorange rate.  WR{k} renders the uncertainty in pseudorange rates for the visible satellites at epoch k.

The spoofed data appended with "outlier" render the same information for the spoofed data.

