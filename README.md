# pod-ishell(Pod shell interactive tool)
useage:
./podIshell 
Commands:
  clear       clear the screen
  cli         Enter shell interactive mode
  desc        Output pod description information
  exec        Send instructions to pod to execute,e: exec <args>
  exit        exit the program
  help        display help
  init        Initialize the pod list
  list        Print pod list information
  pwd         Show home directory
  select      Choose pod and container
  showme      Show current location
  switch      Switch workload, e: switch | switch {ns} {workloadType} {workloadName} {gv}


[help]
Usage of ./podIshell:
  -gv string
    	set group version, e: -gv [apps/v1 | extensions/v1beta1] (default "apps/v1")
  -kubeconfig string
    	set absolute path to kubeconfig file (default "/home/lemon/.kube/config")
  -name string
    	set workload name,e: -name [name]
  -ns string
    	set namespace, e: -ns [namespace] (default "default")
  -t string
    	set workload type,e: -type [deployment|statefulSet|daemonSet]

[example1]
./podIshell -name email-app-server -t deployment
