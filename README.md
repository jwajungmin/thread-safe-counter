# thread-safe-counter

20163421

jwajungmin

This code is compiled in WSL2 (Ubuntu).

You can use these C program by using command 
"time ./tscounter.out [number]" and "time ./tscounter_original.out [number]"

In here, "tscounter_original.out" file means by Mutex and "tscounter.out" file means by Semaphore

By Semaphore

![tscounter](https://user-images.githubusercontent.com/62414463/121784492-21d28880-cbef-11eb-962c-6aea64c17559.png)




By Mutex

![tscounter_original](https://user-images.githubusercontent.com/62414463/121784515-36168580-cbef-11eb-9dbf-23ccfc5382f2.png)

As you can see, by Semaphore was much slower than by Mutex. So I thought it should be used in resource
that obtains a long usage time. 

Despite this shortcomings, there are no crash in critical section by semaphore. So we have to choose wisely for each situation.