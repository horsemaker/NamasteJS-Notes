# How JavaScript Code is executed & Call Stack


<i>The given example had only one function so creation and deletion of execution context seemed simple but what if a program has multiple functions and other functions being invoked within a function? Wondering how the JavaScript engine handles such a tedious task? JavaScript engine manages these things very effectively with the help of **“Call Stack”**.
</i>

### Call stack in JavaScript
- **“Call Stack maintains the order of execution of the execution contexts”**
- In order to maintain the order of execution of the execution contexts and efficiently perform creation and deletion of the execution contexts JavaScript uses **Call Stack**
- Call Stack is also called as:
    - Execution Context Stack
	- Program Stack
	- Control Stack
	- Run time Stack
	- Machine Stack
- The global execution context is present at the base of the stack
- The newly created execution context is placed at the top of the stack and once the execution is completed, it is popped from the stack
- In the given example,the global execution context is at the base of the stack and when the square function is invoked on line number 6, an execution context (E1) is created and placed on the top of the global execution context. Once it’s execution is completed, it is removed from the top of the stack and the control returns back to the global execution context
- Then on line number 7, square function is invoked again so execution context (E2) is created and placed on the top of the stack. Once it’s execution is completed it is popped from the stack and the control moves back to the global execution context
- Once the program is executed completely, global execution context is also popped from the stack and the call stack becomes empty.










