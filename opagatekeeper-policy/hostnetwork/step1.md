Allowing pods to use the "hostNetwork" gives them access to the host machine's network interface. So in case of a compromise, this lets the attacker sniff the traffic going through the host network from the compromised pod.