SOURCE_IMAGE = os.getenv("SOURCE_IMAGE", default='tkg-harborplf.dha-tkgdemo.net/tanzu/spring-sensors-app-source')
LOCAL_PATH = os.getenv("LOCAL_PATH", default='.')
NAMESPACE = os.getenv("NAMESPACE", default='demo')

k8s_custom_deploy(
    'spring-sensors',
    apply_cmd="tanzu apps workload apply -f ./config/workload.yaml --live-update" + \
               " --registry-ca-cert " + "C:\\Users\\dha.8EA48C7-OOBE-01\\tanzu\\all-dha-tkgdemo.net.ca.crt" + \
               " --label apps.tanzu.vmware.com/workload-type=web" + \
               " --local-path " + "./" + \
               " --source-image " + SOURCE_IMAGE + \
               " --namespace " + NAMESPACE + \
               " --yes >/NUL" + \
               " && kubectl get workload spring-sensors --namespace " + NAMESPACE + " -o yaml",
    delete_cmd="tanzu apps workload delete -f ./config/workload.yaml --namespace " + NAMESPACE + " --yes",
    deps=['pom.xml', './target/classes'],
    container_selector='workload',
    live_update = [
        sync('./target/classes', '/workspace/BOOT-INF/classes')
      ]
)

k8s_resource('spring-sensors', port_forwards=["8080:8080"],
            extra_pod_selectors=[{'serving.knative.dev/service': 'spring-sensors'}])
allow_k8s_contexts('full-cluster-admin@full-cluster')



