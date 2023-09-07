## Reaching Definitions Analysis
### Reaching Definitions
A definition d at program point p reaches a point q if there is a path from p to q such that d is not "killed" along the path
- A definition of a variable v is a statement that assigns a value to v
- Translated as: definition of variable v at program point p reaches point q if there is a path from p to q such that no new definition of v appears on that path.
- can be used to detect possible undefined variables.

$D: v = x\ op\ y$ 
This statement "generates" a definition D of variable v and "kills" all the other definitions in the program that define variable v, while leaving the remaining incoming definitions unaffected.
![[Data Flow Analysis Applications-.png]]