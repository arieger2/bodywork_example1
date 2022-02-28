kubectl minio proxy -n minio-operator
kubectl port-forward svc/s3storage-console 9443:9443 -n ml-pipeline
https://localhost:9443/login

{
   "console":[
      {
         "url":"https://minio.ml-pipeline.svc.cluster.local:443",
         "access_key":"alexanderrieger",
         "secret_key":"alexanderrieger",
         "api":"s3v4",
         "path":"auto"
      }
   ]
}

