# Red Hat OpenShift

Red Hat OpenShift is an enterprise Kubernetes platform that provides a consistent hybrid cloud foundation for building, deploying, and scaling containerized applications. OpenShift extends Kubernetes with developer productivity tools, built-in CI/CD pipelines, integrated monitoring and logging, automated cluster management, role-based access control, and security policies. It supports deployments on bare metal, virtual machines, public clouds, and managed OpenShift services (ROSA, ARO, RHOIC).

**URL:** [https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/apis.yml)

## Tags

Containers, Enterprise, Hybrid Cloud, Kubernetes, PaaS, Red Hat

## APIs

### [Red Hat OpenShift Container Platform API](openapi/red-hat-openshift-api-openapi.yml)
The OpenShift Container Platform REST API is a Kubernetes-compatible REST API that extends the core Kubernetes API with OpenShift-specific resources. It provides programmatic access to manage workloads, networking, storage, builds, pipelines, security, and cluster configuration.

**Base URL:** `https://api.cluster.example.com:6443`

- [Documentation](https://docs.openshift.com/container-platform/latest/rest_api/index.html)
- [Getting Started](https://developers.redhat.com/products/openshift/getting-started)
- [OpenAPI](openapi/red-hat-openshift-api-openapi.yml)

### [Red Hat OpenShift Cluster Manager API](openapi/red-hat-openshift-cluster-manager-openapi.yml)
The OpenShift Cluster Manager (OCM) API provides programmatic access to the Red Hat Hybrid Cloud Console for managing OpenShift clusters at scale. Operations include creating, updating, and deleting clusters; managing cluster add-ons; and configuring identity providers.

**Base URL:** `https://api.openshift.com`

- [Documentation](https://api.openshift.com/)
- [OpenAPI](openapi/red-hat-openshift-cluster-manager-openapi.yml)

### Red Hat OpenShift Pipelines (Tekton) API
OpenShift Pipelines is a cloud-native CI/CD solution based on Tekton that runs pipelines as Kubernetes-native CRDs. The API provides resources for defining Tasks, Pipelines, PipelineRuns, TaskRuns, Workspaces, and EventListeners for event-driven pipeline automation.

**Base URL:** `https://api.cluster.example.com:6443/apis/tekton.dev/v1`

- [Documentation](https://docs.openshift.com/container-platform/latest/cicd/pipelines/understanding-openshift-pipelines.html)
- [GitHub](https://github.com/openshift/pipelines-as-code)

### Red Hat OpenShift GitOps (ArgoCD) API
OpenShift GitOps is built on Argo CD and provides a GitOps continuous delivery solution for OpenShift clusters. The API exposes Application, AppProject, ApplicationSet, and Repository CRD resources for declarative cluster state management from Git repositories.

**Base URL:** `https://api.cluster.example.com:6443/apis/argoproj.io/v1alpha1`

- [Documentation](https://docs.openshift.com/container-platform/latest/cicd/gitops/understanding-openshift-gitops.html)
- [GitHub](https://github.com/openshift/gitops-operator)

### Red Hat OpenShift Service Mesh API
Red Hat OpenShift Service Mesh, based on Istio, provides traffic management, security, and observability for microservices. The Service Mesh API exposes Istio CRDs including VirtualService, DestinationRule, Gateway, PeerAuthentication, and AuthorizationPolicy resources.

**Base URL:** `https://api.cluster.example.com:6443/apis/networking.istio.io/v1beta1`

- [Documentation](https://docs.openshift.com/container-platform/latest/service_mesh/v2x/ossm-about.html)

### Red Hat OpenShift Serverless (Knative) API
OpenShift Serverless, based on Knative, enables deploying and managing event-driven serverless workloads on OpenShift. The Serverless API exposes Knative Serving resources for auto-scaling workloads and Knative Eventing resources for event-driven architectures.

**Base URL:** `https://api.cluster.example.com:6443/apis/serving.knative.dev/v1`

- [Documentation](https://docs.openshift.com/serverless/latest/about/about-serverless.html)

### Red Hat OpenShift Service on AWS (ROSA) API
Red Hat OpenShift Service on AWS (ROSA) is a fully managed OpenShift service co-managed by Red Hat and AWS. The ROSA API provides operations for creating and managing ROSA clusters, configuring machine pools, managing identity providers, and monitoring cluster status.

**Base URL:** `https://api.openshift.com/api/clusters_mgmt/v1`

- [Documentation](https://docs.openshift.com/rosa/rosa_architecture/rosa-understanding.html)
- [Getting Started](https://docs.openshift.com/rosa/rosa_getting_started/rosa-getting-started-iam-prerequisites.html)

## Capabilities

### Workflow Capabilities

| Capability | Description |
|-----------|-------------|
| [Cluster Management](capabilities/cluster-management.yaml) | Unified capability combining cluster lifecycle management and OpenShift resource operations (12 MCP tools) |

### Shared Definitions

| File | API |
|------|-----|
| [openshift-api.yaml](capabilities/shared/openshift-api.yaml) | OpenShift Container Platform API |
| [cluster-manager-api.yaml](capabilities/shared/cluster-manager-api.yaml) | OpenShift Cluster Manager API |

## Artifacts

| Type | File |
|------|------|
| OpenAPI | [Container Platform API](openapi/red-hat-openshift-api-openapi.yml) |
| OpenAPI | [Cluster Manager API](openapi/red-hat-openshift-cluster-manager-openapi.yml) |
| JSON Schema | [Project](json-schema/red-hat-openshift-project-schema.json) |
| JSON Structure | [Project Structure](json-structure/red-hat-openshift-project-structure.json) |
| JSON-LD Context | [OpenShift Context](json-ld/red-hat-openshift-context.jsonld) |
| Spectral Rules | [OpenShift Rules](rules/red-hat-openshift-rules.yml) |
| Vocabulary | [OpenShift Vocabulary](vocabulary/red-hat-openshift-vocabulary.yml) |

## Examples

- [Create Project](examples/red-hat-openshift-create-project-example.json)
- [Create Route](examples/red-hat-openshift-create-route-example.json)

## Common Properties

- [Website](https://www.redhat.com/en/technologies/cloud-computing/openshift)
- [Documentation](https://docs.openshift.com/)
- [Pricing](https://www.redhat.com/en/technologies/cloud-computing/openshift/pricing)
- [Blog](https://www.redhat.com/en/blog/channel/red-hat-openshift)
- [GitHub Organization](https://github.com/openshift)
- [Sign Up](https://www.redhat.com/en/technologies/cloud-computing/openshift/try-it)
- [Status](https://status.redhat.com/)
- [Support](https://access.redhat.com/support)
- [Privacy Policy](https://www.redhat.com/en/about/privacy-policy)
- [Terms of Service](https://www.redhat.com/en/about/agreements)
- [Training](https://www.redhat.com/en/services/training-and-certification)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
