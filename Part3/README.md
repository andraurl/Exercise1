# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > *Concurrency means that mulitiple threads can be processed at the same time, but the CPU goes back and fourth between the different threds. Keep in mind that the CPU can only do one thing at the time. Parralelism means that a task can be separated into subtasks that is solved in parralell meaning multiple CPUs handle the problem.*

 ### Why have machines become increasingly multicore in the past decade?
 > *This is the most efficient way to increase the CPU speed. As we are aproching a limit for how much we can increase the clockrate, the solution for still making faster machines is to introduce parralellism and multiple cores.*

 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > *In real life parralelism is happening all the time. If you were to order something on ebay, it would be hopeless if you had to wate in line to make an order. It would be much more natural if you could enter your order erlier so you could leave, than waiting for the server to prioritize you entierly.*

 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > *This is a classical give and take example. It becomes more tricky because you have to make some restrictions on premisions regarding reading and writing to memory. In the example that was codes it shows how terrible things can go if you do not know what is going on.
Things become easier in the way that it comes more natural to program in this way, because this is what we observe in the real life.*

 ### What are the differences between processes, threads, green threads, and coroutines?
 > *A process has its own address memory that no other process can access. All threads is a part of a process?
 Green thread *

 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > *pthread_create() - thread - OS thread
 threading.Thread() - green Thread - OS Thread
 go - Goroutines - michsture of both green threads and coroutines. Changes in runtime*

 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > *A global interpreter lock (GIL) is a mechanism used in computer-language interpreters to synchronize the execution of threads so that only one native thread can execute at a time. An interpreter that uses GIL always allows exactly one thread to execute at a time, even if run on a multi-core processor.

 Locks to one CPU*

 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > *Thread module*

 ### What does `func GOMAXPROCS(n int) int` change?
 > *Sets nr. of CPUs that can be used in the calculation. if n < 1 no change is done.*
