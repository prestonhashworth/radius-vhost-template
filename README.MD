Virtual Hosts dependencies and subdependencies - a virtual host is where header manipulations and key elements of the VIP are configured

1. Routes -these are the request match criteria and the destination for each match. Unspecified match criteria matches all.
    a. Destination List - has a sub match criteria and then references clusters
        i. Clusters - these contain the final endpoints (origin server pools) that allow the definition of origin servers and the ports they receive traffic on and the site references (where applicable)
2. Advertise Policies - these define where the virtual host is advertised as a VIP, their protocol, and port, and optionally a VIP ip and TLS where required
