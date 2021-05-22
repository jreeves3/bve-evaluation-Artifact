# bve-evaluation
Bounded Variable Elimination evaluation on various solver configurations for pigeonhole formulas. (POS21)

## data 
Excel spreadsheet with sheets labeled by Figure.

## formulas
* phpN.cnf - sparse formulas
* phpNfull.cnf - full formulas
* phpNeH.cnf - n=N, h=H, with n+1 variables eliminated as described in the paper

## solvers
* [Kissat](https://github.com/arminbiere/kissat)
* [CaDiCaL](https://github.com/arminbiere/cadical)
* [Maple LCM Dist ChronoBT DL v3 (2019)](http://sat-race-2019.ciirc.cvut.cz/)
* [Maple LCM Dist ChronoBT (2018)](sat2018.forsyte.tuwien.ac.at)
* [Maple LCM Dist (2017)](https://baldur.iti.kit.edu/sat-competition-2017/)

Solvers can be found from their respective years at the [Sat Competition Website](http://satcompetition.org/)

Solvers with StarExec configurations are also attached. Note Maple (2019) can have its step decrement adjusted  manually in sources\core\Solver.cc for each of the three LRB configurations, but this could easily be done by adding more starExec run scripts to the default LRB configuration.

The attached CaDiCaL and Kissat21 have the option --scoredump=1 for outputing variable scores at each conflict.
