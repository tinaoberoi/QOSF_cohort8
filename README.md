QOSF Task cohort 8

## Problem Statement

Task1: Find the primes numbers

Given a positive integer and an list of prime numbers, look for the two prime numbers, that sum the positive number. Consider an appropriate number of qubits and explain why your proposal is valid for all kinds of numbers in case

```
def find_the_primes_numbers (int:number_1, list[int] ,number_2):
     “””
 number_1 : integer value that is the positive number to decompose,
number_2 : integer list that has two prime numbers to add to obtain number_1.
Return the number_a and number_b
     “””

     # use a framework that works with quantum circuits, qiskit, cirq, pennylane, etc. 

      # consider print your quantum circuit,

```

```
Example:

A = find_the_primes_numbers (18,[1,3,5,7,11,13,15])
print(A)

“3,15”
```
## Solution:

- The find_pair function loops through `i+1` for every i (i = 0 to N). And calculate the sum of the numbers using `qadd`. The adder in qadd is implemeted using qft and iqft. 

- The `find_pair` function takes `target sum ` and an `arr` and returns the pair whose sum is equivalent to the target. 

## Example:
```
target = 24
arr = [1,3,5,7,11,13,15]
pair = find_pair (target, arr)
print(f"\n Target Sum {target} can be achieved by sum of : {pair}")

```

```
Target Sum 24 can be achieved by sum of : (11, 13)
```

*Note*: The image of the circuit is stored in file `circuit_img.tex`.

## References:

[Implementing binary adder](https://www.electronics-tutorials.ws/combination/comb_7.html)
[Draper Adder Qiskit](https://qiskit.org/documentation/stubs/qiskit.circuit.library.DraperQFTAdder.html)
[Quantum Adder](https://quantumcomputing.stackexchange.com/questions/32848/trying-to-understand-a-quantum-adder)
[Drapper QFT Adder](https://docs.quantum-computing.ibm.com/api/qiskit/qiskit.circuit.library.DraperQFTAdder)



