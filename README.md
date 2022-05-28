# ACM TOMS Algorithm 857: POLSYS_GLP: a parallel general linear product homotopy code for solving polynomial systems of equations

POLSYS_GLP consists of Fortran 95 modules for finding all isolated solutions of a complex coefficient polynomial system of equations. The package is intended to be used on a distributed memory multiprocessor in conjunction with HOMPACK90 (Algorithm 777), and makes extensive use of Fortran 95-derived data types and MPI to support a general linear product (GLP) polynomial system structure. GLP structure is intermediate between the partitioned linear product structure used by POLSYS_PLP (Algorithm 801) and the BKK-based structure used by PHCPACK. The code requires a GLP structure as input, and although finding the optimal GLP structure is a difficult combinatorial problem, generally physical or engineering intuition about a problem yields a very good GLP structure. POLSYS_GLP employs a sophisticated power series end game for handling singular solutions, and provides support for problem definition both at a high level and via hand-crafted code. Different GLP structures and their corresponding Bezout numbers can be systematically explored before committing to root finding.

 - This code has been re-uploaded with the permission of Dr. Layne Watson.
   All comments and questions should be directed to him (see contact info at
   the bottom of this file).

## Structure and Usage

The original source code, exactly as distributed by ACM TOMS, is included in
the ``src`` directory.
The ``src`` directory also contains its own ``README``, build instructions,
and a test case.
Comments at the top of each subroutine document their proper usage.

## Reference and Contact

To cite this work, use:

```
    @article{algorithm857,
        author = {Su, Hai-Jun and McCarthy, J. Michael and Sosonkina, Masha and Watson, Layne T.},
        title = {Algorithm 857: POLSYS_GLP—a Parallel General Linear Product Homotopy Code for Solving Polynomial Systems of Equations},
        year = {2006},
        volume = {32},
        number = {4},
        journal = {ACM Trans. Math. Softw.},
        pages = {561–579},
        doi = {10.1145/1186785.1186789}
    }
```

Inquiries should be directed to

Layne T. Watson,  
Department of Computer Science, VPI&SU,  
Blacksburg, VA 24061-0106;  
(540) 231-7540;  
ltw@vt.edu  

