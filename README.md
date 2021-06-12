# thread-safe-counter

20163421

jwajungmin

This code is compiled in WSL2 (Ubuntu).

You can use these C program by using command 
"time ./tscounter.out [number]" and "time ./tscounter_original.out [number]"

In here, "tscounter_original.out" file means by Mutex and "tscounter.out" file means by Semaphore


![Semaphore](./github_image/tscounter.png)


![Mutex](./github_image/tscounter_original.png)

As you can see, by Semaphore was much slower than by Mutex. So I thought it should be used in resource
that obtains a long usage time. 

Despite this shortcomings, there are no crash in critical section by semaphore. So we have to choose wisely for each situation.