# cs214-assignment-3-fork-and-exec---returned-solved
**TO GET THIS SOLUTION VISIT:** [CS214 Assignment 3-fork and exec – Returned Solved](https://www.ankitcodinghub.com/product/cs214-assignment-3-fork-and-exec-returned-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;90752&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS214 Assignment 3-fork and exec - Returned Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
<div class="column"></div>
</div>
<div class="layoutArea">
<div class="column">
&nbsp;

Base Program

We want a program that word-wraps several les and concatenates them. We have a working executable for ww, but no source code, so we cannot modify it for our purposes.

This almost works:

<pre>    $ cat file1 file2 file3 | ./ww 80
</pre>
Unfortunately, it may result in the last paragraph of one le being combined with the rst paragraph of the next. (Exercise: Why is this?)

Instead, write a program wcat that takes a positive integer and one or more le names as arguments. For each le, it will use fork to spawn a child process, and the child process will use execl or execv to execute ww for a single le, using the provided integer as the page width. Ensure that a blank line separates the last paragraph of one le from the rst paragraph of the next.

Note that the child process shares standard output with the parent process, so ww will print to the terminal without any work on your part.

Enhancement I

</div>
</div>
<div class="layoutArea">
<div class="column">
https://sakai.rutgers.edu/portal/site/f55b6385-2252-4de5-a0e1-6b8fe3227eeb/tool/5b736e6b-8b6b-4963-af7f-8ab2a622a40c?panel=Main 1/3

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
1/24/22, 2:45 PM sakai.rutgers.edu : CS 214 — Spring 2021 : Assignments

Before invoking ww, make sure that the le name does not refer to a directory. If it does, print a message to standard error and skip the le. Return EXIT_FAILURE once all processing is complete.

Enhancement II [1 point]

Check the exit status of ww (that is, the exit status of the child process). If the status is not EXIT_SUCCESS, then wcat should return EXIT_FAILURE once all processing is complete.

Enhancement III

Simply printing a newline between les may result in consecutive blank lines if one of the input les is empty or contains only whitespace. Use the technique described in class to arrange a pipe so that wcat can read the output of ww and copy it to standard output, but also detect whether there was any output at all.

You may assume that ww is well-behaved and will output either (a) at least one non-blank line, or (b) nothing, and that its output will not begin or end with a blank line.

Note 1

Use a macro to hard-code the location of ww. For example,

#ifndef WWPATH

#dene WWPATH “/ilab/users/abc123/bin/ww” #endif

When testing, it is ne to use something like “./ww” as the path as long as you only run wcat in the same directory as ww.

Note 2

When using pipe, be aware that open le descriptors are duplicated between the parent and child processes. In particular, the read end will not report EOF until both the parent and child have closed the write end.

Note 3

Recall that dup2 lets us assign an open le to a specic le descriptor. For example, dup2(x, 1) will make standard output refer to the same le that x refers to.

Note 4

You may use write or fprintf to write to standard error. For write, use le descriptor 2. For fprintf or other f* functions use the global variable stderr.

&nbsp;

</div>
</div>
</div>
