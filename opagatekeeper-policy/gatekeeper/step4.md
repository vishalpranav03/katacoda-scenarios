Now that the policy has been implemented, we'll see if it has been done properly.

We have two files. One file - **violation.yaml**, which violates the enforced policy and the other file - **non-violation.yaml**, which does not.

We can conclude that the policy has been enforced correctly if the violation.yaml file gets denied and the non-violation.yaml file does not.

## violation.yaml
`kubectl apply -f https://raw.githubusercontent.com/vishalpranav03/opa-gatekeeper-policies/main/OPA%20Gatekeeper/Prohibit%20host%20path/deployment-violation.yaml`{{execute}}

This will get denied.

## non-violation.yaml
`kubectl apply -f https://raw.githubusercontent.com/vishalpranav03/opa-gatekeeper-policies/main/OPA%20Gatekeeper/Prohibit%20host%20path/deployment-non-violation.yaml`{{execute}}

This will not get denied.