# Notes on Istio helm chart

We've forked the istio helm chart to make several modifications, listed here. To repackage the chart, navigate to the root directory and run make.  

# Change log

These are changes made to the standard istio chart. 

1. Change boolean logic so installing CRDs can be turned off (`istio/templates/crds.yaml`) 
2. Support post-upgrade as a hook for istio-security-post-install job (`istio/charts/security/templates/create-custom-resources-job.yaml`)
