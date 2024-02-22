docker login -u  jiraroth
dckr_pat_ICCT-n7tJF9aZCRlw4GOQ-ExPA8

docker build -t local_jiraroth:1.0 .

Rename Image :
docker tag  local_jiraroth:1.0 jiraroth/custom-nginx-registry:2.0

docker push jiraroth/custom-nginx-registry:2.0jiraroth

docker pull jiraroth/custom-nginx-registry:2.0

docker run -d -p 8085:80 jiraroth/custom-nginx-registry:2.0