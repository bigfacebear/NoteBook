# TACC

## Stampede2

[**Stampede2 User Guide**](https://portal.tacc.utexas.edu/user-guides/stampede2#introduction)

### Access the Compute Nodes

#### Three basic ways to access the compute nodes:

1. [Submit a **batch job** using the `sbatch` command](https://portal.tacc.utexas.edu/user-guides/stampede2#running-sbatch). This directs the scheduler to run the job unattended when there are resources available. Until your batch job begins it will wait in a [queue](https://portal.tacc.utexas.edu/user-guides/stampede2#running-queues). You do not need to remain connected while the job is waiting or executing. See [Running Jobs](https://portal.tacc.utexas.edu/user-guides/stampede2#running) for more information. Note that the scheduler does not start jobs on a first come, first served basis; it juggles many variables to keep the machine busy while balancing the competing needs of all users. **The best way to minimize wait time is to request only the resources you really need**: the scheduler will have an easier time finding a slot for the two hours you need than for the 48 hours you unnecessarily request.
2. Begin an [**interactive session** using `idev` or `srun`](https://portal.tacc.utexas.edu/user-guides/stampede2#running-idev). This will log you into a compute node and give you a command prompt there, where you can issue commands and run code as if you were doing so on your personal machine. An interactive session is **a great way to develop, test, and debug code**. When you request an interactive session, the scheduler submits a job on your behalf. You will need to remain logged in until the interactive session begins.
3. Begin an [interactive session using **ssh**](https://portal.tacc.utexas.edu/user-guides/stampede2#running-ssh) to connect to a compute node on which you are **already running a job**. This is a good way to open a second window into a node so that you can **monitor a job while it runs**.