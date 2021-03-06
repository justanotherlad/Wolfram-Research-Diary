----------
###### Title: WSS'2020 - Day 3
###### Date: 30-06-2020
----------
&nbsp;


> Started looking into my selected 5 potential-project topics (suggested by Stephen Wolfram) in depth:

> - ###### Make a Framework for Zero Knowledge Proofs:
>
> WL has a good framework for public key encryption, digital signatures, etc. Design functions that implement zero knowledge proofs in similar ways.
https://www.moneycontrol.com/news/technology/ey-releases-zero-knowledge-proof-blockchain-transaction-technology-to-the-public-domain-3851381.html
https://www.ey.com/en_gl/news/2019/04/ey-releases-zero-knowledge-proof-blockchain-transaction-technology-to-the-public-domain-to-advance-blockchain-privacy-standards
>
> https://github.com/EYBlockchain/ZKPChallenge 
> [[ [Re: SNARKS
> I see it like this:
>
> We have to imagine blockchain named XX that uses STARKs.
> It will use an interactive or a non-interactive zk-proof (they say STARK can be either).
> If it’s non-interactive we could do it silently inside BlockchainTransactionSign/Submit for BlockchainBase -> XX.
> Alternatively, if it’s interactive (thus, has to receive something from the blockchain XX) or we just want to expose that we’re doing it we could have a separate function like BlockchainZKProofConstruct which yields a ZKProof[] object / ByteArray which then becomes an input to BlockchainTransactionSubmit.
>
> Assuming we won’t have to implement from scratch all the math from their whitepaper.
> 
> Dariia]]]]

&nbsp;



> - ###### Implement Level-Index Arithmetic for Very Large Numbers:
>
> https://mrob.com/pub/perl/hypercalc.html
> https://en.wikipedia.org/wiki/Symmetric_level-index_arithmetic


&nbsp;


> - ###### Symbolic Manipulation of Tetration
>
> Get a symbolic representation for results: https://mrob.com/pub/math/largenum-3.html#hyper4


&nbsp;


> - ###### Implement Transfinite Arithmetic
>
> Set up symbolic transformation rules for Cantor’s transfinite arithmetic. Probably need to have TransfinitePlus, etc., but get to these using upvalues.


&nbsp;


> - ###### Collect & Implement Additional Axiomatic/Formal Systems
>
> AxiomaticTheory has a variety of standard axiom systems from mathematics. Implement more of them, e.g. for specific types of algebraic systems, but also for systems from theoretical computer science, philosophical logic, etc.


--------------------------------------------------------------------------------------------------------------------------------------------------------------
> ##### Self-Study time:

> - Topic (2)
>
> ***Doubts*** : HYpercalc stores and manipulates numbers using a level-index format; as such it can go far beyond the limits of bc, dc, MACSYMA/maxima,Mathematica and Maple, all of which use a bigint library (arbitrary- precision arithmetic).
> 
> ***Notes***: one question is always, how far can the approximations be made.
There's always the tower of power paradox...so with small errors or differences, you would require large digits for precision/approximation, but there's a limit to that we can have, and there's always gonna be a larger number which can have an even smaller error which requires further more number of digits to store the exact error
> 
> ***Doubt***: Only difference between Hypercalc and Mathematics, as I see, is that, Hypercalc uses level-index arithmetic representations for really large numbers. Otherwise, the approximations and errors for really large numbers both in Mathematica and HYpercalc uses arbitraty-precision arithmetic algorithm.
Isn't it Too trivial?
Don't understand why not implemented yet? 
ONly work, implement the JS code in mathematica to represent large numbers using some level-index arithmetic representation
>
> ***NOtes***: Interesting Algorithm: https://mrob.com/pub/seq/a092188.html
To calculate upto N digits of a power tower in 10^N steps at max

-------------------------------------------------------------------------
&nbsp;


> - Topic (3): Tetration
>
> ***Note***: https://community.wolfram.com/groups/-/m/t/1139667?p_p_auth=4xTC6sCX (handy blog by WSC student)
>
> ***Note***:  When a number x and 10 are coprime, it is possible to compute the last m decimal digits of   x^x^x^...(a times) using Euler's theorem, for any integer m.
>
> ***Note***: Interesting visual simulations of complex realms of Tetration: https://en.wikipedia.org/wiki/Tetration#/media/File:Tetration_escape.png
>
> ***Note***: Infinite Tetration converges for numbers in a certain interval
>
>
> ***Doubt for Stephen Wolfram***: Doubt: What does the project title name *Symbolic Manupulations* of Tetration mean?
("Get a symbolic representation for results" !?!?!?!?)

> READ UP OVERVIEWS ABOUT GODEL'S INCOMPLETENESS THEOREM
> ASKED [JONATHAN GORARD](https://education.wolfram.com/summer/school/alumni/2017/gorard/) (Physics Track Head, Masters in Maths, King's College, London) ABOUT GOOD BOOKS TO START READING ABOUT AXIOMATIC SET THEORY/ LOGIC THEORY. SUGGESTED ***Kleene's "Introduction to Metamathematics"*** and  slightly dry, ***van Dalen's "Logic and Structure"*** 

> SHO HINARA SUGGESTED ***Russel’s “Artificial Intelligence - A modern approach”*** 

-------------------------------------------------------------------------------

> Mentor meeting for about 25mins at 2.00am at night. Doubt removal session.

&nbsp;
> ###### [Next Day](Day4.md)
