# operatingsystem-assignment-2-solved
**TO GET THIS SOLUTION VISIT:** [OperatingSystem Assignment 2 Solved](https://www.ankitcodinghub.com/product/operatingsystem-assignment-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91419&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;OperatingSystem Assignment 2 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
1 Exec family system call and basic IPC using signals API.

The first exercise tries to familiarize you with exec family system calls and signals API. In this program you are required to create a child process, lets call it S1. You need to save the PID of the process just created using a local variable. The body of process S1, should register a signal handler for SIGTERM which could be raised by any other process, using the kill() system call.

Thereafter, following the creation of process S1 the main (parent) program should fork two more child processes, ST and SR. Both ST and SR should reg- ister signal handler for the signal SIGALRM. Both should setup appropriate timers using the setitmerval() system call (that should invoke a timer for both the processes, individually) at every predecided interval (e.g. 1s, 2s, etc.).

Note 1: Functionality of SR: Corresponding to SR, the SIGLARM handler should read a random number from the CPU using the the RDRAND instruc- tion (using inline assembly). Then, SR needs to enqueue the random number and the SIGTERM and deliver it to S1’s SIGTERM handler (using kill() sys- tem call). S1’s SIGTERM handler should print the said random number.

Note 2: Functionality of ST: We require a similar SIGALRM handler for ST. The ST process should read the CPU timestamp counter (using inline as- sembly to run RDTSC instruction), and coverts into a human readable string (i.e. representing the current date and time), at every interval. The interval can be set using the setitimer() system call, that raises then SIGALRM signal everytime the timeout elapses, that is trapped by an appropriate signal handler. The random number should be obtained (using the inline RDTSC instruction), in the SIGALRM handler function. Much like SR, the ST’s SIGALRM handler should enqueue the string along with the SIGTERM signal and deliver it to S1’s SIGTERM handler (using kill()), that should print it.

Note 3: Using exec family system calls to launch the two programs SR and ST: Also, it must be noted that the entire functionality of ST and SR

1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
should be embodied in two individual programs. In other words, there should be two executable programs E1 and E2 corresponding to SR and ST respectively, that should accept the PID of S1 as an argument. These programs, i.e. E1 and E2, must be launched from SR and ST respectively using the exec family of system calls, especially those that allow launching programs with arguments.

What to submit/rubric.

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
<div class="layoutArea">
<div class="column">
1.

2.

3. 4.

</div>
<div class="column">
All the three program sources, corresponding to the main() function, pro- gram E1 (which is invoked from SR) and E2 (which is invoked in ST). These programs should compile successfully. [Successfully compilation of all the three programs: 25 points. No points for programs that do not compile.]

Correctly functioning programs achieving the required functionalities. [All the three programs correctly functioning: 25 points. Some of the programs working correctly, but not all: 12.5 points. Programs that seem logically correct but none of them work as expected (provided, it compiled successfully: 6.25 points.]

A single Makefile to compile the above three programs.[Fully function- ing Makefile: 5 points.]

README/Write-up describing the program logic used for achieving the above (no more than one page).[10 points]

Kernel memory copy (kernel 2d memcpy()) (To- tal points: 70).

</div>
</div>
<div class="layoutArea">
<div class="column">
This exercise aimed to test your understanding how system calls work. You need to write a system call, kernel 2d memcpy(), which copies one 2-D float- ing point matrix to another. You would require using kernel functions like

copy from user() and copy from user() to read data bytes from user space and write back to user space. In other words, this is a version of memcpy() that relies on the kernel to do the necessary copy operations, which are otherwise usually done directly in the user space (using the standard C library routines).

What to submit/rubric.

<ol>
<li>The diff between the stock kernel and the kernel with your appropriate system call. This diff could be patched into the stock kernel code so as to achieve the required functionality (i.e. the system call) and used eventually. [Successfully compilation of the patched kernel: 50 points. No partial points.]</li>
<li>A sample program to test the above system call. In the program you could hard-wire the source 2-D matrix (i.e. no need to take input from user at runtime or via a file). [Program that correctly calls the system call with all the appropriate parameters and does the copy, provided (1) above works i.e.:10 points. Program compiles (as well as (1) above works), but copying is unsuccessful: 5 points.]</li>
<li>README/Write-up describing the program logic used for achieving the above (no more than one page). [10 points]
2
</li>
</ol>
</div>
</div>
</div>
