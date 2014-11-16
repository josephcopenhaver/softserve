FEATURES:

1. forks using the same environmental config as the original
2. forks using the same command line argumrnts as the original
3. the parent process will not yield control of network resources until the child process signals that it is ready to take control
4. parent process will not terminate until all executing tasks terminate
5. the module will supply a registration mechanism to enumerate network resources/currently serving ports/services
6. the module will provide inspection as to whether or not the current process is a fork or a parent (although such knowledge is not entirely useful given tha nature of the module's intent)
7. a fork process shall not take control of existing network resources until after the parent process has been informed and confirmed of the forked process' ownership of said resources