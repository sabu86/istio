# istio
To create a simple gateway for our node-docker app.
# kubectl create ns chaos
# kubectl apply -f nodedoc.yaml -n chaos
# kubectl apply -f service_nodedoc.yaml -n chaos
# At this point the node-docker should be accessible via port 8000 and the url will be http://localhost:8000/test
# kubectl apply -f istiogateway.yaml -n chaos
# http://localhost/test works fine


# RUNNING THE NETWORK ABORT CHAOS EXPERIMENT
# Created the network.yaml file
# chaos run network.yaml (At this point the experiment fails with error [2020-11-17 16:46:44 ERROR]  => failed: KeyError: 'subset', 
[2020-11-17 16:46:43 INFO] Validating the experiment's syntax
[2020-11-17 16:46:44 INFO] Experiment looks valid
[2020-11-17 16:46:44 INFO] Running experiment: What happens if we abort responses
[2020-11-17 16:46:44 INFO] Steady-state strategy: default
[2020-11-17 16:46:44 INFO] Rollbacks strategy: default
[2020-11-17 16:46:44 INFO] Steady state hypothesis: The app is healthy
[2020-11-17 16:46:44 INFO] Probe: app-responds-to-requests
[2020-11-17 16:46:44 INFO] Probe: app-responds-to-requests
[2020-11-17 16:46:44 INFO] Probe: app-responds-to-requests
[2020-11-17 16:46:44 INFO] Probe: app-responds-to-requests
[2020-11-17 16:46:44 INFO] Probe: app-responds-to-requests
[2020-11-17 16:46:44 INFO] Steady state hypothesis is met!
[2020-11-17 16:46:44 INFO] Playing your experiment's method now...
[2020-11-17 16:46:44 INFO] Action: abort-failure
# [2020-11-17 16:46:44 ERROR]   => failed: KeyError: 'subset'
[2020-11-17 16:46:44 INFO] Pausing after activity for 1s...
[2020-11-17 16:46:45 INFO] Steady state hypothesis: The app is healthy
[2020-11-17 16:46:45 INFO] Probe: app-responds-to-requests
[2020-11-17 16:46:45 INFO] Probe: app-responds-to-requests
[2020-11-17 16:46:45 INFO] Probe: app-responds-to-requests
[2020-11-17 16:46:45 INFO] Probe: app-responds-to-requests
[2020-11-17 16:46:45 INFO] Probe: app-responds-to-requests
[2020-11-17 16:46:45 INFO] Steady state hypothesis is met!
[2020-11-17 16:46:45 INFO] Let's rollback...
[2020-11-17 16:46:45 INFO] No declared rollbacks, let's move on.
[2020-11-17 16:46:45 INFO] Experiment ended with status: completed

