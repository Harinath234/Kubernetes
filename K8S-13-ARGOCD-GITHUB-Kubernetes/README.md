
Deploymentfiles has to be in github

GitHub contains Kubernetes manifests such as Deployment and Service YAML files. Argo CD continuously monitors the Git repository and syncs any changes to the Kubernetes cluster. When the Deployment manifest is updated (for example, with a new image version), Kubernetes performs a rolling update and creates new pods. The Service of type LoadBalancer exposes the application externally by routing traffic to the running pods.
