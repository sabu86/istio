# istio
To create a simple gateway for our node-docker app.
# kubectl create ns chaos
# kubectl apply -f nodedoc.yaml -n chaos
# kubectl apply -f service_nodedoc.yaml -n chaos
# At this point the node-docker should be accessible via port 8000 and the url will be http://localhost:8000/test
# kubectl apply -f istiogateway.yaml -n chaos
