## Reaching Definitions Analysis
### Reaching Definitions
A definition d at program point p reaches a point q if there is a path from p to q such that d is not "killed" along the path
- A definition of a variable v is a statement that assigns a value to v
- Translated as: definition of variable v at program point p reaches point q if there is a path from p to q such that no new definition of v appears on that path.
- can be used to detect possible undefined variables.

$D: v = x\ op\ y$ 
This statement "generates" a definition D of variable v and "kills" all the other definitions in the program that define variable v, while leaving the remaining incoming definitions unaffected.

![image.png](https://raw.githubusercontent.com/0xDkXy/image/master/202309071829256.png?token=ANK274EJ3GBK3LXT2LQZ2QLE7GTEQ)
### Example
![image.png](https://raw.githubusercontent.com/0xDkXy/image/master/202309071831490.png?token=ANK274B6Y3CCTP6F3T5UYZ3E7GTNA)
### Why this iterative algorithm can finally stop
fixed point / monotonicity

## Live Variable Analysis
Live variables analysis tells whether the value of variable v at program point p could be used along some path in CFG starting at p. If so, v is live at p; otherwise, v is dead at p.

- information of live variables can be used for register allocations. e.g., at some point all registers are full and we need to use one, then we should favor using a register with a dead value.
### Algorithm of Live Variable Analysis
![image.png](https://raw.githubusercontent.com/0xDkXy/image/master/202309071842390.png?token=ANK274EYD364JJTLJP4JUCDE7GUVQ)
### Example
![image.png](https://raw.githubusercontent.com/0xDkXy/image/master/202309071850618.png?token=ANK274HDOEU2TBIRXCOIVILE7GVUM)
**Notice:** in the iteration 1, when calculate the $in[b]$ of B2, the m is not in the $use[b2]$ because it was defined in the previous line.
## Available Expression Analysis
An expression $x\ op\ y$ is available at program point p if:
1. all paths from the entry to p *must* pass through the evaluation of $x\ op\ y$, 
2. after the last evaluation of $x\ op\ y$, there is no redefinition of $x\ op\ y$
