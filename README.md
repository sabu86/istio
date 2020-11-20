# istio
To create a simple gateway for our node-docker app.
# kubectl create ns chaos
# kubectl apply -f nodedoc.yaml -n chaos
# kubectl apply -f service_nodedoc.yaml -n chaos
# At this point the node-docker should be accessible via port 8000 and the url will be http://localhost:8000/test
# kubectl apply -f istiogateway.yaml -n chaos
# http://localhost/test works fine

# Created the network-rollback.yaml file
# RUNNING THE NETWORK ABORT CHAOS with retries EXPERIMENT after applying the istio-repeater.yaml to my cluster.
# chaos run network-rollback.yaml (At this point the experiment fails since the retires section isnt working) 
