# kubeschemas

`kubeschemas` contains massive public maintained kubernetes json schema (1500+ types), including all kubernetes buitin resource types, well known CRDs and kubernetes related configuration file.

## kubernetes.nvim

These schemas are used by [kubernetes.nvim](https://github.com/imroc/kubernetes.nvim).

## kubernetes buitin resource types

All Kubernetes buitin resource types are supported (e.g. `Deployment`, `ConfigMap`, `StatefulSet` and etc).

## CRDs

A lot of public well known CRDs are supported (generated by [kubeschema](https://github.com/imroc/kubeschema)):

CRDs from cloud vendor:

- [Tencent Cloud TKE](https://cloud.tencent.com/product/tke)
- [Huawei Cloud CCE](https://www.huaweicloud.com/product/cce.html)
- [Google Cloud GKE](https://cloud.google.com/kubernetes-engine)
- [AWS EKS](https://aws.amazon.com/eks/)

CRDs from open source project:

- [Gateway API](https://gateway-api.sigs.k8s.io/guides/#install-standard-channel)
- [MCS API](https://github.com/kubernetes-sigs/mcs-api/tree/master/config/crd)
- [Istio](https://istio.io/latest/docs/setup/install/helm/)
- [Envoy Gateway](https://github.com/envoyproxy/gateway/tree/main/charts/gateway-helm/crds)
- [Cilium](https://github.com/cilium/cilium/tree/main/pkg/k8s/apis/cilium.io/client/crds)
- [APISIX](https://github.com/apache/apisix-helm-chart/tree/master/charts/apisix-ingress-controller/crds)
- [Higress](https://github.com/alibaba/higress/tree/main/helm/core/crds)
- [Traefik](https://github.com/traefik/traefik-helm-chart/tree/master/traefik/crds)
- [Kong](https://github.com/Kong/kubernetes-configuration/tree/main/config/crd)
- [cert-manager](https://github.com/cert-manager/cert-manager/tree/master/deploy/crds)
- [opentelemetry-operator](https://github.com/open-telemetry/opentelemetry-helm-charts/tree/main/charts/opentelemetry-operator/conf/crds)
- [Ambassador Edge Stack](https://www.getambassador.io/docs/edge-stack/latest/tutorials/getting-started)
- [karmada](https://github.com/karmada-io/karmada/tree/master/charts/karmada/_crds) and [karmada-operator](https://github.com/karmada-io/karmada/tree/master/charts/karmada-operator/crds)
- [clusternet](https://github.com/clusternet/clusternet/tree/main/manifests/crds)
- [spark-operator](https://github.com/kubeflow/spark-operator/tree/master/charts/spark-operator-chart/crds)
- [flink-operator](https://github.com/apache/flink-kubernetes-operator/tree/main/helm/flink-kubernetes-operator/crds)
- [karpenter](https://github.com/kubernetes-sigs/karpenter/tree/main/pkg/apis/crds)
- [kruise](https://openkruise.io/docs/installation/), [kruise-rollout](https://openkruise.io/rollouts/installation) and [kruise-game](https://openkruise.io/kruisegame/installation)
- [argo-cd](https://github.com/argoproj/argo-cd/tree/master/manifests/crds), [argo-workflows](https://github.com/argoproj/argo-workflows/tree/main/manifests/base/crds), [argo-rollouts](https://github.com/argoproj/argo-rollouts/tree/master/manifests/crds) and [argo-events](https://github.com/argoproj/argo-events/tree/master/manifests/base/crds)
- [tekton-operator](https://github.com/tektoncd/operator/blob/main/docs/install.md), [tekton-pipeline](https://github.com/tektoncd/pipeline/blob/main/docs/install.md), [tekton-triggers](https://github.com/tektoncd/triggers/blob/main/docs/install.md)
- [zalando postgres-operator](https://github.com/zalando/postgres-operator/tree/master/charts/postgres-operator/crds) and [CrunchyData postgres-operator](https://github.com/CrunchyData/postgres-operator-examples/tree/main/helm/install/crds)
- [OPA gatekeeper](https://github.com/open-policy-agent/gatekeeper/tree/master/charts/gatekeeper/crds)
- [velero](https://github.com/vmware-tanzu/velero/tree/main/config/crd)
- [knative-operator](https://knative.dev/docs/install/operator/knative-with-operators/#install-the-knative-operator), [knative-serving](https://knative.dev/docs/install/yaml-install/serving/install-serving-with-yaml/#install-the-knative-serving-component) and [knative-eventing](https://knative.dev/docs/install/yaml-install/eventing/install-eventing-with-yaml/#install-knative-eventing)
- [volcano](https://github.com/volcano-sh/volcano/tree/master/config/crd)
- [linkerd](https://linkerd.io/2.17/getting-started/#step-3-install-linkerd-onto-your-cluster)
- [agones](https://agones.dev/site/docs/installation/install-agones/yaml/)
- [crane](https://github.com/gocrane/helm-charts/tree/main/charts/crane/crds)
- [tidb-operator](https://github.com/pingcap/tidb-operator/tree/master/manifests/crd)
- [prometheus-operator](https://github.com/prometheus-community/helm-charts/tree/main/charts/kube-prometheus-stack/charts/crds/crds)
- [kuberhealthy](https://github.com/kuberhealthy/kuberhealthy/tree/master/deploy/helm/kuberhealthy/crds)
- [k3s](https://github.com/k3s-io/k3s)
- [mongodb atlas-operator](https://github.com/mongodb/helm-charts/tree/main/charts/atlas-operator-crds), [mongodb community-operator](https://github.com/mongodb/helm-charts/tree/main/charts/community-operator-crds) and [mongodb enterprise-operator](https://github.com/mongodb/helm-charts/tree/main/charts/enterprise-operator/crds)
- [dragonfly-operator](https://raw.githubusercontent.com/dragonflydb/dragonfly-operator/refs/heads/main/manifests/crd.yaml)
- [fluxcd](https://github.com/fluxcd/flux2/blob/main/manifests/crds/kustomization.yaml)
- Rancher(TODO)
- KubeSphere(TODO)
- OpenShift(TODO)

## Configuration File

Some kubernetes related configuration file schemas are also included:

- [Kubernetes Configuration APIs](https://kubernetes.io/docs/reference/config-api/) (e.g. kubeconfig, kubeadm/kubelet/kube-proxy/kube-apiserver/controller-manager/kube-scheduler configuration files and etc)
- [Kind Configuration](https://kind.sigs.k8s.io/docs/user/configuration/)
- [K3D Config File](https://k3d.io/stable/usage/configfile/)

## Contributing

You can add more schemas by running `kubeschema dump --index` in the root directory of git repo to dump schemas from current kubernetes cluster.

PRs are welcome!
