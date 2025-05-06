# comp429-529-assignment-2-parallel-nqueens-solved
**TO GET THIS SOLUTION VISIT:** [COMP429-529 Assignment 2-Parallel-nqueens Solved](https://www.ankitcodinghub.com/product/comp429-529-assignment-2-parallel-nqueens-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96022&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP429-529 Assignment 2-Parallel-nqueens Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
Description

In this assignment you will parallelize an n-queens solver using OpenMP. This application will help you exercise your knowledge in task parallelism. You are provided with the serial version of this application and you must develop your parallel implementation on top of it. Be aware that each part requires you to collect performance data with several runs so allow yourself enough time to conduct those experiments before the deadline.

PART II: Parallel N-Queens Solver

In the second part of this assignment, you are asked to parallelize a serial n-queens solver with OpenMP. Similar to Part I, you are provided with a serial n-queens solver code, which takes an n-queens problem as an input and finds all possible solutions from it. We are using a brute force search for searching for all possible solutions to the problem.

For a given nxn chessboard, the idea is to generate every possible move by trying each cell withinacolumni,suchthat0 ≤ i &lt; n,andthen,testingtoseewhetherqueenplacement in the cell satisfies the n-queens’ constraint (no chess queen in the board/matrix can kill each other). After finding a cell in column i that satisfies the constraints, the program moves to column i+1 to find another queen placement in that column. This process is repeated recursively until the last column n – 1.

A solution is printed after there is a queen in every column of the matrix with the n-queens’ constraint being satisfied. After finding a solution by placing the last queen in column n – 1, the program backtracks to the previous column n-2 to try other cells in the column and moves forward again to find another placement of the last queen in column n – 1. This backtracking process is repeated so that when the program backtracks to a column i, all possible placements in columns j, s.t. i &lt; j &lt; n, have been found. By the time the backtracking process completes, all possible solutions for n-queens problem have been found.

</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
Part-II-A Task Parallelism COMP 429/529 ( ): AssignmPenAtR1T-PIaIr:tP2ARALLEL N-QUEENS SOLVER Part-II-A Task Parallelism

In the first part, you are required to parallelize the n-queens solver with task parallelism. Similar to the serial version, the parallel version is expected to find all possible solutions to a given n-queens problem.

Part-II-B Task Parallelism with Cutoff

The first implementation results in too many tasks in the system which can easily degrade the performance. As a result, you may not experience any speedup or very disappointing speedup. In this part, you will implement an optimization to improve the performance of the parallel code by using a cutoff parameter to limit the number of parallel tasks in your code. To limit task generations, beyond certain depth in the call-path tree of the recursive function, switch to the serial execution and do not generate tasks. This depth is determined by the cutoff parameter you choose.

Part-II-C Task Parallelism with Early Termination

In this part, you will start working from the parallel code that you implemented in Part-II-A. You are going to modify the code so that it stops after finding one solution instead of all possible solutions. To make a fair performance comparison, you should also modify the serial version so that it also stops after finding one solution to n-queens.

Experimental Study

You must collect the performance data on the KUACC cluster. Plot your data as figures and include them in your report along with some description for your observations and explanations. Do the experiments with the input size of 14 and with thread count of 1, 2, 4, 8, 16, and 32 threads unless stated otherwise..

a) Scalability Test

Perform the same strong scaling experiment on your implementation.

<ul>
<li>For the parallel code from Part-II-A and B, you must compute the speedup with respect to the given serial n-queens solver.</li>
<li>For the parallel code from Part-II-C, you must compute the speedup with respect to a modified version of the given serial n-queens solver that also terminates after finding one valid solution.
b) Thread Binding Test

Perform the strong scaling experiment under 2 different thread mapping schemes; compact mapping and scatter mapping. If you run the previous test with compact mapping, then you just need to repeat the same test with scatter mapping. See lecture 8 for more explanations.
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
Student Name: Page 2 of 5

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
COMP 429/529 ( ): Assignment 1-Part 2 ENVIRONMENT c) Tests on n-queens Problems of Different Sizes

For this test, you will report the running times of the parallel code from Part-II-A on n- queens problems of different sizes by using 32 threads. The sizes that you will test are 13, 14, and 15.

Environment

Even if you develop and test your implementations on your local machine or on the computer labs on campus, you must collect performance data on the KUACC cluster.

<ul>
<li>Accessing KUACC outside of campus requires VPN. You can install VPN through this link: https://my.ku.edu.tr/faydali-linkler/</li>
<li>A detailed explanation is provided in http://login.kuacc.ku.edu.tr/ to run programs in the KUACC cluster. In this document, we briefly explain it for the Unix-based systems. For other platforms you can refer to the above link.</li>
<li>In order to log in to the KUACC cluster, you can use ssh (Secure Shell) in a command line as follows: The user name and passwords are the same as your email account.</li>
</ul>
<ol>
<li>1 &nbsp;bash$ ssh $&lt;$username$&gt;$@login.kuacc.ku.edu.tr</li>
<li>2 &nbsp;bash$ ssh dunat@login.kuacc.ku.edu.tr //example</li>
</ol>
<ul>
<li>The machine you logged into is called login node or front-end node. You are not supposed to run jobs in the login node but only compile them at the login node. The jobs run on the compute nodes by submitting job scripts.</li>
<li>To run jobs in the cluster, you have to change your directory to your scratch folder and work from there. The path to your scratch folder is</li>
</ul>
1 bash$ cd /scratch/users/username/

• To submit a job to the cluster, you can create and run a shell script with the following command:

1 bash$ sbatch &lt;scriptname&gt;.sh

A sample of the shell script is provided in Blackboard along with the assignment folder. In the website of the KUACC cluster, a lot more details are provided.

• To copy any file from your local machine to the cluster, you can use the scp (secure copy) command on your local machine as follows:

<ol>
<li>1 &nbsp;scp -r &lt;filename&gt; &lt;username&gt;@login.kuacc.ku.edu.tr:/kuacc/users/&lt;username&gt;/</li>
<li>2 &nbsp;scp -r src_folder dunat@login.kuacc.ku.edu.tr:/kuacc/users/dunat/ //example
-r stands for recursive, so it will copy the src folder with its subfolders.
</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
Student Name: Page 3 of 5

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
Grading COMP 429/529 ( ): Assignment 1-Part 2 ENVIRONMENT • Likewise, in order to copy files from the cluster into the current directory in your local

machine, you can use the following command on your local machine:

<ol>
<li>1 &nbsp;scp -r &lt;username&gt;@login.kuacc.ku.edu.tr:/kuacc/users/&lt;username&gt;/fileToBeCopied ./</li>
<li>2 &nbsp;scp -r dunat@login.kuacc.ku.edu.tr:/kuacc/users/dunat/src_code ./ //example</li>
</ol>
• To compile the assignment on the cluster, you can use the GNU or Intel compiler. The compilation commands and flags for the compilers are provided in a Makefile in the assignment folder. Before using the compilers, you firstly need to load their module if they are not already loaded as follows:

<ol>
<li>1 &nbsp;bash$ module avail //shows all available modules in KUACC</li>
<li>2 &nbsp;bash$ module list //list currently loaded modules.</li>
<li>3 &nbsp;bash$ module load intel/ipsxe2019-u1ce //loads Intel compiler</li>
<li>4 &nbsp;bash$ module load gcc/7.2.1/gcc //loads GNU compiler</li>
</ol>
<ul>
<li>If you have problems compiling or running jobs on KUACC, first check the website provided by the KU IT. If you cannot find the solution there, you can always post a question on Blackboard.</li>
<li>Don’t leave the experiments on KUACC to the last minutes of the deadline as the machine gets busy time to time. Note that there are many other people on campus using the cluster.
Grading
</li>
</ul>
</div>
</div>
</div>
