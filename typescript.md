#### Dynamic vs Static
Static: define the type of variable

e.g. `int a;`

Pros:

 * Code is documented, or self-documenting.
 * Because of that, there are less errors, less bugs. Engineers will catch errors earlier.
 * Helps with autocompletion.

Cons:

 * More code. Another layer of complexity. 

Dynamic: no need to define

e.g. `let a = 100;`


---
#### Strong vs Weak
Strong type doesn't allow coercion.

---
ReasonML vs TypeScript vs Elm vs Flow

Use if:

 * If project is growing larger and larger
 * You want code to be self-documenting
 * You have band-width to train others / JRs

---

:closed_book: Type refinement - be sure to enforce certain data exists

```
if (data) {
  // then do stuff
}
```