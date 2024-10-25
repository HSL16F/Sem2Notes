Determine behaviour of object.
State-dependent object responds with respect to object's state
State-intendent object: Object responds regardless of objects state
State machines explore state dependent objects and have the ability to model complex behaviour. For complex state-dependent objects, it is less common for business information, but more common for communication and control applications.
Generally thought of as having a flow of information.
**Transition Actions:**
	Action/object that  does something when transition occurs
**Guard:**
	Pre-condition to transition, only happen if guard/trigger is true
When object is in State A, if trigger event occurs and guard is true, then perform action behaviour and transition object to State B.
ADD TRANSITION IMAGE
There can exist substates in the sates, these are called nested states.
A substate inherits transitions of its superstate (enclosing state)
A substate, a series of operations can occur, essentially its a state machine inside of a given state
Pseudostate is one with some conditional branch, evaluates guards of triggle in outgoing transition with only one outcome.
There can be two or more outgoing transitions, and can use pre-defined else guards if no other are true.

#### Examples:
![[Pasted image 20241024174359.png]]
![[Pasted image 20241024174409.png]]
![[Pasted image 20241024174425.png]]
![[Pasted image 20241024174449.png]]
![[Pasted image 20241024174605.png]]