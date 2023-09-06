## Howto use Validated Pattern as described on https://hybrid-cloud-patterns.io/
we are using the multicloud-gitops pattern as an example.

-Fork the template repo from https://github.com/mbaldessari/multicloud-gitops

- Git clone your forked repo locally, example 
❯ git clone https://github.com/<username>/multicloud-gitops

- Check if you are on the right branch with 
❯ git branch -a

- If you want to change branche type
❯ git checkout dgw

- Check your OpenShift | Kubernetes context is set right, ie are you sourcing the right kubeconfig file
❯ oc whoami -c

- Switch to your branch within the multicloud-gitops directory and call ./pattern.sh make install
❯ ./pattern.sh make install

Loggin into your OpenShift console under 'Operators >> Installed Operators' this should then show the follwing operators installed:
- Red Hat OpenShift GitOps
- Validated Patterns Operator



