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
 > *Your answer here*
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > *Your answer here*
 
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > *Your answer here*
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > *Your answer here*
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > *Your answer here*
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > *Your answer here*
