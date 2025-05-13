# podman-sample

# command sample

## run nginx container
podman -d --name my-nginx -p 8081:80 -v ./nginx_html:/usr/share/nginx/html:ro nginx

## show runing containers
podman ps

## stop container
podman stop ${CONTAINER_NAME}

## rm container
podman rm ${CONTAINER_NAME}

## dump kubernetes manifest
podman generate kube ${CONTAINER_NAME}

## create pod from kubenetes manifest
podman play kube ${MANIFEST_FILE_PATH}

