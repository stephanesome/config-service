# Deploy
k8s_yaml(['k8s/deployment.yml', 'k8s/service.yml'])

# Build
docker_build('stephanesome/config-service', '.')

# Manage
k8s_resource('config-service', port_forwards=['8888'])
