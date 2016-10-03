# Falcon
This project combines RDMA and Paxos. The raw evaluation results are available here: [performance on replicated programs](https://docs.google.com/spreadsheets/d/1_lMG-KMgHAQldZoaiktpokGsiDU1_43BrXGY0BVZkWY/edit#gid=0), [consensus latency breakdown](https://docs.google.com/spreadsheets/d/1_lMG-KMgHAQldZoaiktpokGsiDU1_43BrXGY0BVZkWY/edit#gid=738955580), [comparison with DARE](https://docs.google.com/spreadsheets/d/1_lMG-KMgHAQldZoaiktpokGsiDU1_43BrXGY0BVZkWY/edit#gid=1107443132) and [scalability evaluation](https://docs.google.com/spreadsheets/d/1_lMG-KMgHAQldZoaiktpokGsiDU1_43BrXGY0BVZkWY/edit#gid=1775362239).
  
OS: Ubuntu 14.04.02 64bit.
## How to run
### Install the dependencies for the program
Use $RDMA_ROOT/RDMA/mk to download and install the dependencies for the program.
### Install the applications
We have prepared all the Makefiles for you in each application's directory.
### Run the evaluation framework
For example, to run Redis hooked by Falcon, just go to $RDMA_ROOT/eval and run `python eval.py -f redis-output.cfg`. After that, you can collect the results by `cd current`.
