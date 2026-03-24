
--> create 1-deploy_AC_V1.yaml
kubectl apply -f 1-deploy_AC_V1.yaml
kubectl get all
kubectl describe deploy fb-deploy

--> create 2-deploy_VC_v2.yaml
kubectl apply -f 2-deploy_VC_v2.yaml
kubectl get all
kubectl describe deploy fb-deploy

kubectl rollout undo deploy fb-deploy
kubectl get po --watch
kubectl get all
kubectl describe deploy fb-deploy
kubectl rollout history deploy fbdeploy

kubectl rollout pause deploy fb-deploy
kubectl rollout resume deploy fb-deploy

