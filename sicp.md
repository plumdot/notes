# Structure and Interpretation of Computer Programs

> To use an analogy, if SICP were about automobiles, it would be for the person who wants to know how cars work, how they are built, and how one might design fuel-efficient, safe, reliable vehicles for the 21st century. The people who hate SICP are the ones who just want to know how to drive their car on the highway, just like everyone else.

[Peter Norvig](https://www.amazon.com/review/R403HR4VL71K8)

---

### Helpful resources

[Install Racket](https://www.youtube.com/watch?v=-EFrmOa0bP0)

[MIT/Scheme User Manual](https://www.gnu.org/software/mit-scheme/documentation/mit-scheme-user.pdf)

---

To run a file:
```
> racket file_to_run.rkt
```

---


## 1: Building Abstractions with Procedures

### 1.1: 

 * Expressions
 * Conditional Expressions and Predicates
 * Applicative order vs Normal order
    * Normal order is "fully expand and then reduce"
    * Applicative order is is "evaluate the arguments and then apply"

### 1.2: Procedures and the Processes They Generate 

 * A procedure is a pattern for the local evolution of a computational process.
 * Recursive:
   ```
    (define (factorial n)
        (if (= n 1)
        1
        (* n (factorial (- n 1))))
   ```
 * Iterative:
    ```
    (define (factorial n)
        (define (iter product counter)
        (if (> counter n)
        product
        (iter (* counter product)
            (+ counter 1))))
        (iter 1 1))
    ```
 * Tail Recursive - Iteration can be expressed using the ordinary procedure call mechanism, so that special iteration constructs are useful only as syntactic sugar.


## 2: Building Abstractions with Data
## 3: Modularity, Objects, and State
## 4: Metalinguistic Abstraction
## 5: Computing with Register Machines

###