# Binary Big Bang

Any BTech student have seen binary numnbers at least once in his/ her life. Here,
I am proposing a crazy Idea based on these binary patterns.

## Background

As we all know, computer can understand only binary combinations. If we write
all possible binary combinations containing `n-bits` in a single column then
we don't see any pattern. <br/>
Ex: 3 bit binary numbers <br/>
|   000    |
| -------- |
|   001    |
| -------- |
|   010    |
| -------- |
|   011    |
| -------- |
|   100    |
| -------- |
|   101    |
| -------- |
|   110    |
| -------- |
|   111    |
| -------- |
<br/>
But if we write same `n-bits` binary combinations in following format then we
start seeing some pattern. Ex: Same 3 bit binary combinations<br/>
|   0 ones  |   1 ones  |   2 ones  |   3 ones  |
| --------- | --------- | --------- | --------- |
|   000     |   001     |   011     |   111     |
| --------- | --------- | --------- | --------- |
|           |   010     |   101     |           |
| --------- | --------- | --------- | --------- |
|           |   100     |   110     |           |
| --------- | --------- | --------- | --------- |
<br/>
Now this table shows that only 50% patterns are original and rest 50% can be
derived (complement). Even if see closely then only 25% patterns are original
and rest 75% can derived.

## Idea: Binary Big Bang

We have established that only 25% binary patterns are original. With this it can
be said that any n bit binary pattern can be represented by `(n / 4)` bit
patterns (here it is assumed that encoding and decoding can be done in some
way. **How? (And that is the question to universe. Let's hope it has answer.)**).
So, we can form some kind of recursive equation here: <br/>

```
pattern (n) = pattern (n / 4)
```

The above equation can be extended till the point until n become 1.

>
> **Note:** When n become 1, we have 2 binary pattern (0, 1). But using qubits,
> we can reach to 1 pattern (n = 1 / 2). And that's the binary big bang.
>

## Conclusion

We can reach n = 1, i.e. 2 binary patterns using current tech (VLSI/ ULSI). So,
if this idea works then any information can be represented in 1 bit.<br/>
Ex: A 4GB Bluray movie can be saved in 1 bit.