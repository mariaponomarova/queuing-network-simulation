Project description

I. Closed Queuing network simulation (17 pt)

Build a simulator to capture the following system and answer the questions below. A total of N=40 jobs circulate in different parts of the systems: CPU, disk, and resting area. There is one CPU and two disks, one slow and one fast. Each job starts at the CPU station and takes an average of 2 seconds. After CPU, a job fetches the data from the disk, needing an average of 3000 disk cycles. There are two possible choices of disks, fast and slow, which have a speed of 1000 cycles per second and 100 cycles per seconds, respectively. After the disk station, the job can rest for 15 seconds on average. The figure below gives an overview of the system:

The choices of distributions are up to you. You are welcomed to try different distributions to answer the following questions and assess the impact of different variants.
 
Questions:
1. (3p) What will be the maximal system throughput in terms of number of jobs, given two different load balancing strategies for sending jobs between the fast and slow disk? You need to come up with two load balancing strategies and compare them. 
2. (3p) What will the system throughput and average response time of a job be if a faster CPU is used? Say, CPU time is reduced to 1 seconds on average and the rest of the system remains the same.
3. (3p) What will the system throughput and average response time of a job be if a second fast disk is added? Again, you need to compare the throughput under two different load balancing strategies.
4. (3p) What will the system throughput and average response time of a job be if a faster CPU is used and a second fast disk is added? And, you use the better load balancing strategies out of two you propose in the first question?
5. (5pt) If you can answer all the above questions with different number of N and plot them in the following style:
 

II. Open Queuing network simulation (8 pt)

The second part of the project is to make an open-queuing network simulator, where the jobs arrive from the outside following Poisson processes with the rate of lambda. The system is shown as the following figure:

Each job needs to go to the CPU, following an exponential distribution with a mean of 10 jobs per second, and then proceeds by either one of the disks. There are two disks, each of which has an exponentially-distributed processing time. The fast disk has a processing rate of 12 jobs per second and the slow disk has the rate of 9 jobs per second. The number of buffer spaces in each queue is infinite.

Questions:
1. (4pt) Use your simulator to find the maximum sustainable throughput of such a system in terms of number of jobs. Support your answer with simulation results.
2. (4pt) Find out the average response times for following cases over three arrival rates of your choice: case (i) - a single queue in front of fast and slow disk; case (ii) - a separate queue for each disk, jointly applying the shortest queue load balancing strategy when sending the jobs from the CPU to disk.

