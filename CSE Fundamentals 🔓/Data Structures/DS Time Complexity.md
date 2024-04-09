# Phitron
### Introduction
- ✔️ Time complexity not measure general time. Because it's will be take different times value based on machine performance.
- ✔️ So, how to measure time complexity? Measurement uses take program steps.
- ✔️ Time complexity measurement technique or formula is called **Big O Notation**. 
- ✔️ Big O Notation Formula => **O(steps(grammer,input)).**
- ✔️ Every statements is called **steps**.
- ✔️ Assginment, loop, Comparison, Condition are more have steps.
- ✔️ So many steps take so many time complexity.
- ✔️ Grammer:
	- Always declare for worst case.
	- Ignore the constants.
	- Always avoid minimun task, accepted maximum task.
	- Always measure with input(n) value, not constant value.
	- If different input value, then take both but valuable will be after input only maximum.
- ==Time Complexity becomes from loop== .
- ==Constant steps always 1 O(1). It's time complexity 0.

### How time is calculated from time complexity
- Online judgement server maximum times take 1second and beyond this time execute task maximum $10^8$ .
- $10^8$ is not sure all server, somewhere plus, somewhere minus, that's why it's take reasonable $10^7$. So that, you not faced **time limit execed**.
- always remove constant value.
- always use loop and maximum value.
- constant steps task always **O(1)**.
### How Time is Determined?
- 1s = 10$^8$ = 10$^7$
- 2s = 10$^7$ * 2
- 3s = 10$^7$ * 3
- ......
- 10$^8$ = 10s
- 10$^9$ = 100s
- ......
- O(1) = max = 10$^7$ = 1s = it's can increased that's time
- O(N) = max = 10$^7$ = 1s (it's can increased or decresed using +,-)
- O(logN) = max= 10$^{18}$  = 1s = it's can increased or decreased using (*,/)
- O(NlogN)
- O(sqrt(n)) = max = 10$^{14}$ = 1s = it's can be that times task of root.
- O(n\*n) = max = 10$^3$ = 1s = it's can use nested loop
## Grammer
- Always calculate for worst case;
- Ignore the constants value;
- Determine time complexity based on input value;
- Complexity is comming from loop;
- If not exist any loop, it's complexity will be O(1);
- If have multiple loop, it's complexity will be maximum input value loop;
- If have multiple loop, but input value is different, it's complexity wil be summation of input value;
- If multiple input value then will be addition all of.
## Kinds OF Time Complexity:
- O(1);
	- not have loop;
	- not have input;
- O(N);
	- single or multiple loop;
	- but input value same or not; if not same O(N+M);
	- i += k; k = 1 is worst case
	- i -= k; k = 1 is worst case
- O(logN);
	- single or multiple loop;
	- but input value same;
	- i \*= k; k = 2 is worst case
	- i /= k; k =2 is worst case
- O(NlogN)
	- single or multiple loop;
	- but input value not same;
	- i\*i;
	- i < root(n);
- O(N\*N)
	- single or multipel value
	- two nested loop;
