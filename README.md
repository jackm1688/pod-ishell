# pod-ishell(Pod shell interactive tool) <br/>
useage:<br/>
./podIshbell <br/>
Commands:
  clear       clear the screen<br/>
  cli         Enter shell interactive mode<br/>
  desc        Output pod description information<br/>
  exec        Send instructions to pod to execute,e: exec <args><br/>
  exit        exit the program<br/>
  help        display help<br/>
  init        Initialize the pod list<br/>
  list        Print pod list information<br/>
  pwd         Show home directory<br/>
  select      Choose pod and container<br/>
  showme      Show current location<br/>
  switch      Switch workload, e: switch | switch {ns} {workloadType} {workloadName} {gv}<br/>
<br/>
<br/>
[help]<br/>
Usage of ./podIshell:<br/>
  -gv string<br/>
    	set group version, e: -gv [apps/v1 | extensions/v1beta1] (default "apps/v1")<br/>
  -kubeconfig string<br/>
    	set absolute path to kubeconfig file (default "/home/lemon/.kube/config")<br/>
  -name string<br/>
    	set workload name,e: -name [name]<br/>
  -ns string<br/>
    	set namespace, e: -ns [namespace] (default "default") <br/>
  -t string<br/>
    	set workload type,e: -type [deployment|statefulSet|daemonSet]<br/>

<br/>
<br/>
[example1]<br/>
./podIshell -name email-app-server -t deployment<br/>
