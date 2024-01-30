# push_swap (125/100)

**push_swap** is a project at 42 School that involves sorting stacks of integers using specific operations. The goal is to implement an algorithm that sorts the stack with the minimum number of operations.

## Features
- Custom implementation of a stack sorting algorithm (based on the Turk Algorithm).
- Supports sorting integers using stack manipulation operations (push, rotate, rrotate and swap even if I barely used the latter).
- Optimized for efficiency and minimal number of operations.
- An integrated (and somewhat basic) checker. (bonus)

## Usage
1. Clone the repository:
   <pre>
   git clone https://github.com/Thawnder/push_swap.git
   </pre>
2. Compile the push_swap program:
   <pre>
   make
   </pre>
3. Run the push_swap program with a list of integers as arguments:
   <pre>
   ./push_swap 3 1 5 4 2
   </pre>
   This will display the list of operations to sort the integers.
4. To run the checker, use a pipe after the push_swap and use the same list as argument.
   <pre>
    ./push_swap 3 1 5 4 2 | ./checker 3 1 5 4 2
   </pre>
   If the sorting instructions for list1 don't match with list2, the checker will return KO. Else, it will return OK.

## Example
<pre>
$ ./push_swap 3 1 5 4 2
sa
ra
ra
pb
pb
ra
ra
pa
pa
ra
</pre>

## Notes
- The push_swap program sorts integers using specific stack manipulation operations for list a, or list b, or both (`sa`, `sb`, `ss`, `pa`, `pb`, `ra`, `rb`, `rr`, `rra`, `rrb`, `rrr`).
- The output displays the sequence of operations to sort the integers.
