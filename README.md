This repository contains script for policy as code that contains policy reinforcement on the Kubernetes pods and validate them while creating if they pass by the policy checks adhered by the security and compliance.
It has 4 files :
1. clusterpolicy.yaml : This is the mail yaml which enforces the policy using Kyverno tool and governs the creation of the pods mandating the cpu and memory request limits.
2. invalid_pod.yaml : This limits the pod creation without mandatory limits being set which does not allow the Kuberntes pods to be created ,this hals the pod creation by any automated process hence governing the cimpliance standards.
3. limit_violating_pod.yaml : This file shows how policy as code is limiting the pod creation in absence of the mandatory request and pods that doesnt align with the policy.
4. valid_pod.yaml : This shows creation of the valid pod which passes the policy governing tool and hence creates the pods as requested.
