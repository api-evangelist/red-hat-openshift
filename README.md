# Red Hat OpenShift (red-hat-openshift)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Red Hat OpenShift is an enterprise Kubernetes platform that provides a consistent hybrid cloud foundation for building, deploying, and scaling containerized applications. OpenShift extends Kubernetes with developer productivity tools, built-in CI/CD pipelines, integrated monitoring and logging, automated cluster management, role-based access control, and security policies. It supports deployments on bare metal, virtual machines, public clouds, and managed OpenShift services (ROSA, ARO, RHOIC). The OpenShift REST API exposes hundreds of Kubernetes and OpenShift-specific resource types organized into API groups for workload management, networking, storage, security, builds, pipelines, and cluster configuration.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- PaaS
- Red Hat

## Timestamps

- **Created:** 2026-03-26
- **Modified:** 2026-05-19

## APIs

### Red Hat OpenShift Container Platform API

The OpenShift Container Platform REST API is a Kubernetes-compatible REST API that extends the core Kubernetes API with OpenShift-specific resources. It provides programmatic access to manage workloads (Pods, Deployments, DeploymentConfigs, StatefulSets), networking (Routes, Ingress, Services, NetworkPolicies), storage (PersistentVolumes, StorageClasses), builds (BuildConfigs, ImageStreams), pipelines (Tekton Pipelines, PipelineRuns), security (SecurityContextConstraints, OAuth, RoleBindings), and cluster configuration. The API is versioned and organized into API groups served at /apis/{group}/{version}.

- **Human URL:** [https://docs.openshift.com/container-platform/latest/rest_api/index.html](https://docs.openshift.com/container-platform/latest/rest_api/index.html)
- **Base URL:** `https://api.cluster.example.com:6443`

#### Tags

- Builds
- Cluster Management
- Containers
- Kubernetes
- Networking
- Workloads

#### Properties

- [Documentation](https://docs.openshift.com/container-platform/latest/rest_api/index.html)
- [Getting Started](https://developers.redhat.com/products/openshift/getting-started)
- [OpenAPI](openapi/red-hat-openshift-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/red-hat-openshift-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Red Hat OpenShift Cluster Manager API

The OpenShift Cluster Manager (OCM) API provides programmatic access to the Red Hat Hybrid Cloud Console for managing OpenShift clusters at scale. Operations include creating, updating, and deleting clusters; managing cluster add-ons; configuring identity providers and role bindings; monitoring cluster health and metrics; and managing subscriptions and quotas. The API is used by the OCM CLI and web console.

- **Human URL:** [https://api.openshift.com/](https://api.openshift.com/)
- **Base URL:** `https://api.openshift.com`

#### Tags

- Cluster Management
- Cloud
- Hybrid Cloud
- Multi-Cluster
- Subscriptions

#### Properties

- [Documentation](https://api.openshift.com/)
- [OpenAPI](https://api.openshift.com/openapi) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/red-hat-openshift-cluster-manager-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/red-hat-openshift-cluster-manager.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-cluster-manager.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Red Hat OpenShift Pipelines (Tekton) API

OpenShift Pipelines is a cloud-native CI/CD solution based on Tekton that runs pipelines as Kubernetes-native CRDs. The API provides resources for defining Tasks (individual steps), Pipelines (task graphs), PipelineRuns (pipeline executions), TaskRuns, Workspaces, TriggerTemplates, and EventListeners for event-driven pipeline automation. All pipeline resources are managed through the Kubernetes API server using the tekton.dev API group.

- **Human URL:** [https://docs.openshift.com/container-platform/latest/cicd/pipelines/understanding-openshift-pipelines.html](https://docs.openshift.com/container-platform/latest/cicd/pipelines/understanding-openshift-pipelines.html)
- **Base URL:** `https://api.cluster.example.com:6443/apis/tekton.dev/v1`

#### Tags

- CI/CD
- Kubernetes
- Pipelines
- Tekton

#### Properties

- [Documentation](https://docs.openshift.com/container-platform/latest/cicd/pipelines/understanding-openshift-pipelines.html)
- [Git Hub](https://github.com/openshift/pipelines-as-code)
- [Postman Collection](collections/red-hat-openshift-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/red-hat-openshift-cluster-manager.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-cluster-manager.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Red Hat OpenShift GitOps (ArgoCD) API

OpenShift GitOps is built on Argo CD and provides a GitOps continuous delivery solution for OpenShift clusters. The API exposes Application, AppProject, ApplicationSet, and Repository CRD resources for declarative cluster state management from Git repositories. The ArgoCD API also includes a REST gRPC-gateway API for direct interaction with the ArgoCD server.

- **Human URL:** [https://docs.openshift.com/container-platform/latest/cicd/gitops/understanding-openshift-gitops.html](https://docs.openshift.com/container-platform/latest/cicd/gitops/understanding-openshift-gitops.html)
- **Base URL:** `https://api.cluster.example.com:6443/apis/argoproj.io/v1alpha1`

#### Tags

- ArgoCD
- CI/CD
- GitOps
- Kubernetes

#### Properties

- [Documentation](https://docs.openshift.com/container-platform/latest/cicd/gitops/understanding-openshift-gitops.html)
- [Git Hub](https://github.com/openshift/gitops-operator)
- [Postman Collection](collections/red-hat-openshift-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/red-hat-openshift-cluster-manager.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-cluster-manager.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Red Hat OpenShift Service Mesh API

Red Hat OpenShift Service Mesh, based on Istio, Kiali, Jaeger, and Prometheus, provides traffic management, security, and observability for microservices. The Service Mesh API exposes Istio CRDs including VirtualService, DestinationRule, ServiceEntry, Gateway, PeerAuthentication, AuthorizationPolicy, and Telemetry resources for configuring service-to-service communication, mutual TLS, and distributed tracing policies.

- **Human URL:** [https://docs.openshift.com/container-platform/latest/service_mesh/v2x/ossm-about.html](https://docs.openshift.com/container-platform/latest/service_mesh/v2x/ossm-about.html)
- **Base URL:** `https://api.cluster.example.com:6443/apis/networking.istio.io/v1beta1`

#### Tags

- Istio
- Kubernetes
- Service Mesh
- Traffic Management

#### Properties

- [Documentation](https://docs.openshift.com/container-platform/latest/service_mesh/v2x/ossm-about.html)
- [Postman Collection](collections/red-hat-openshift-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/red-hat-openshift-cluster-manager.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-cluster-manager.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Red Hat OpenShift Serverless (Knative) API

OpenShift Serverless, based on Knative, enables deploying and managing event-driven serverless workloads on OpenShift. The Serverless API exposes Knative Serving resources (Service, Route, Configuration, Revision) for auto-scaling workloads and Knative Eventing resources (Broker, Trigger, Channel, Subscription, EventSource) for event-driven architectures. Resources are managed through the serving.knative.dev and eventing.knative.dev API groups.

- **Human URL:** [https://docs.openshift.com/serverless/latest/about/about-serverless.html](https://docs.openshift.com/serverless/latest/about/about-serverless.html)
- **Base URL:** `https://api.cluster.example.com:6443/apis/serving.knative.dev/v1`

#### Tags

- Event-Driven
- Knative
- Kubernetes
- Serverless

#### Properties

- [Documentation](https://docs.openshift.com/serverless/latest/about/about-serverless.html)
- [Postman Collection](collections/red-hat-openshift-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/red-hat-openshift-cluster-manager.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-cluster-manager.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Red Hat OpenShift Service on AWS (ROSA) API

Red Hat OpenShift Service on AWS (ROSA) is a fully managed OpenShift service co-managed by Red Hat and AWS. The ROSA API, exposed through the OCM service, provides operations for creating and managing ROSA clusters, configuring machine pools, managing identity providers, setting up private link connectivity, and monitoring cluster status. ROSA clusters also expose the full OpenShift API endpoint after provisioning.

- **Human URL:** [https://docs.openshift.com/rosa/rosa_architecture/rosa-understanding.html](https://docs.openshift.com/rosa/rosa_architecture/rosa-understanding.html)
- **Base URL:** `https://api.openshift.com/api/clusters_mgmt/v1`

#### Tags

- AWS
- Cloud
- Managed Service
- OpenShift

#### Properties

- [Documentation](https://docs.openshift.com/rosa/rosa_architecture/rosa-understanding.html)
- [Getting Started](https://docs.openshift.com/rosa/rosa_getting_started/rosa-getting-started-iam-prerequisites.html)
- [Postman Collection](collections/red-hat-openshift-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/red-hat-openshift-cluster-manager.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/red-hat-openshift-cluster-manager.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.redhat.com/en/technologies/cloud-computing/openshift)
- [Documentation](https://docs.openshift.com/)
- [Pricing](https://www.redhat.com/en/technologies/cloud-computing/openshift/pricing)
- [Blog](https://www.redhat.com/en/blog/channel/red-hat-openshift)
- [GitHub Organization](https://github.com/openshift)
- [Sign Up](https://www.redhat.com/en/technologies/cloud-computing/openshift/try-it)
- [Status Page](https://status.redhat.com/)
- [Support](https://access.redhat.com/support)
- [Privacy Policy](https://www.redhat.com/en/about/privacy-policy)
- [Terms of Service](https://www.redhat.com/en/about/agreements)
- [Training](https://www.redhat.com/en/services/training-and-certification)
- [OpenAPI](openapi/red-hat-openshift-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/red-hat-openshift-cluster-manager-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [J S O N L D Context](json-ld/red-hat-openshift-context.jsonld)
- [JSON Schema](json-schema/red-hat-openshift-project-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/red-hat-openshift-project-structure.json)
- [Spectral Ruleset](rules/red-hat-openshift-rules.yml)
- [Vocabulary](vocabulary/red-hat-openshift-vocabulary.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
