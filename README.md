# Kubernetes - Up and Running

## Description
This repository is capturing my work accomplished and practiced through the [Kubernetes Tutorial](https://www.youtube.com/watch?v=X48VuDVv0do). For the actual explaintation refer the video.

## Getting Started
1. Populate the MongoDB secrets as the secrets need to be in K8s clusters before being referenced by MongoDB with:
`kubectl apply -f mongo-secret.yaml`
2. Verify the secrets were created:
`kubectl get secret`
3. To create both the MongoDB and the MongoDB service. Apply the deployment:
`kubectl apply -f mongo.yaml`
4. ConfigMap must also be present in K8s cluster, before referencing it further:
`kubectl apply -f mongo-configmap.yaml`
5. Apply MongoDB Express:
`kubectl apple -f mongo-express.yaml`
6. You can access MongoDB Express with:
`minikube service mongo-express-service`

