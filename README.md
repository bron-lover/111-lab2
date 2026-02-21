# You Spin Me Round Robin

In this lab, I implemented a Round Robin CPU scheduler, mimicing how processes share the CPU using a fixed time
quantum length. I did this by mainly using a queue comprised of a doubly linked list, correctly dispatching the
next process, and preempting when a particular process had reached the quantum length. Going a little deeper
into how I actually implemented this, I used a while loop, where each iteration represented one clock cycle and
used temporary variables to keep track of timestamps, response time, waiting time, etc. During all this, I
calculated and retunred the average of the response and waiting time.

## Building

```shell
make
```

## Running

cmd for running: ./rr

```shell
./rr processes.txt 3

Output:
Average waiting time: 7.00
Average response time: 2.75
```

results

```shell
python -m unittest

Output:
Ran 2 tests in 0.450s

OK

```

## Cleaning up

```shell
make clean
```
