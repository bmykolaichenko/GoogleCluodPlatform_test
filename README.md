# GoogleCluodPlatform_test

gcloud projects add-iam-policy-binding galvanic-sphinx-305710 \
    --member="serviceAccount:bmykolaichenko@galvanic-sphinx-305710.iam.gserviceaccount.com" \
    --role="roles/owner"

gcloud iam service-accounts add-iam-policy-binding \
bmykolaichenko@galvanic-sphinx-305710.iam.gserviceaccount.com \
    --member="serviceAccount:galvanic-sphinx-305710.svc.id.goog[cnrm-system/cnrm-controller-manager]" \
    --role="roles/iam.workloadIdentityUser"

kubectl --namespace service apply -f enable-sql.yml

kubectl --namespace service apply -f db.yml 

helm create name 

tree 

helm install my-release  prometheus-community/kube-prometheus-stack

kubectl --namespace default get pods -l "release=my-release"

