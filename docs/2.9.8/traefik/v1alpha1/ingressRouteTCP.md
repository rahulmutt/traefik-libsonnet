---
permalink: /2.9.8/traefik/v1alpha1/ingressRouteTCP/
---

# traefik.v1alpha1.ingressRouteTCP

"IngressRouteTCP is the CRD implementation of a Traefik TCP Router."

## Index

* [`fn new(name)`](#fn-new)
* [`obj metadata`](#obj-metadata)
  * [`fn withAnnotations(annotations)`](#fn-metadatawithannotations)
  * [`fn withAnnotationsMixin(annotations)`](#fn-metadatawithannotationsmixin)
  * [`fn withClusterName(clusterName)`](#fn-metadatawithclustername)
  * [`fn withCreationTimestamp(creationTimestamp)`](#fn-metadatawithcreationtimestamp)
  * [`fn withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)`](#fn-metadatawithdeletiongraceperiodseconds)
  * [`fn withDeletionTimestamp(deletionTimestamp)`](#fn-metadatawithdeletiontimestamp)
  * [`fn withFinalizers(finalizers)`](#fn-metadatawithfinalizers)
  * [`fn withFinalizersMixin(finalizers)`](#fn-metadatawithfinalizersmixin)
  * [`fn withGenerateName(generateName)`](#fn-metadatawithgeneratename)
  * [`fn withGeneration(generation)`](#fn-metadatawithgeneration)
  * [`fn withLabels(labels)`](#fn-metadatawithlabels)
  * [`fn withLabelsMixin(labels)`](#fn-metadatawithlabelsmixin)
  * [`fn withName(name)`](#fn-metadatawithname)
  * [`fn withNamespace(namespace)`](#fn-metadatawithnamespace)
  * [`fn withOwnerReferences(ownerReferences)`](#fn-metadatawithownerreferences)
  * [`fn withOwnerReferencesMixin(ownerReferences)`](#fn-metadatawithownerreferencesmixin)
  * [`fn withResourceVersion(resourceVersion)`](#fn-metadatawithresourceversion)
  * [`fn withSelfLink(selfLink)`](#fn-metadatawithselflink)
  * [`fn withUid(uid)`](#fn-metadatawithuid)
* [`obj spec`](#obj-spec)
  * [`fn withEntryPoints(entryPoints)`](#fn-specwithentrypoints)
  * [`fn withEntryPointsMixin(entryPoints)`](#fn-specwithentrypointsmixin)
  * [`fn withRoutes(routes)`](#fn-specwithroutes)
  * [`fn withRoutesMixin(routes)`](#fn-specwithroutesmixin)
  * [`obj spec.routes`](#obj-specroutes)
    * [`fn withMatch(match)`](#fn-specrouteswithmatch)
    * [`fn withMiddlewares(middlewares)`](#fn-specrouteswithmiddlewares)
    * [`fn withMiddlewaresMixin(middlewares)`](#fn-specrouteswithmiddlewaresmixin)
    * [`fn withPriority(priority)`](#fn-specrouteswithpriority)
    * [`fn withServices(services)`](#fn-specrouteswithservices)
    * [`fn withServicesMixin(services)`](#fn-specrouteswithservicesmixin)
    * [`obj spec.routes.middlewares`](#obj-specroutesmiddlewares)
      * [`fn withName(name)`](#fn-specroutesmiddlewareswithname)
      * [`fn withNamespace(namespace)`](#fn-specroutesmiddlewareswithnamespace)
    * [`obj spec.routes.services`](#obj-specroutesservices)
      * [`fn withName(name)`](#fn-specroutesserviceswithname)
      * [`fn withNamespace(namespace)`](#fn-specroutesserviceswithnamespace)
      * [`fn withPort(port)`](#fn-specroutesserviceswithport)
      * [`fn withTerminationDelay(terminationDelay)`](#fn-specroutesserviceswithterminationdelay)
      * [`fn withWeight(weight)`](#fn-specroutesserviceswithweight)
      * [`obj spec.routes.services.proxyProtocol`](#obj-specroutesservicesproxyprotocol)
        * [`fn withVersion(version)`](#fn-specroutesservicesproxyprotocolwithversion)
  * [`obj spec.tls`](#obj-spectls)
    * [`fn withCertResolver(certResolver)`](#fn-spectlswithcertresolver)
    * [`fn withDomains(domains)`](#fn-spectlswithdomains)
    * [`fn withDomainsMixin(domains)`](#fn-spectlswithdomainsmixin)
    * [`fn withPassthrough(passthrough)`](#fn-spectlswithpassthrough)
    * [`fn withSecretName(secretName)`](#fn-spectlswithsecretname)
    * [`obj spec.tls.domains`](#obj-spectlsdomains)
      * [`fn withMain(main)`](#fn-spectlsdomainswithmain)
      * [`fn withSans(sans)`](#fn-spectlsdomainswithsans)
      * [`fn withSansMixin(sans)`](#fn-spectlsdomainswithsansmixin)
    * [`obj spec.tls.options`](#obj-spectlsoptions)
      * [`fn withName(name)`](#fn-spectlsoptionswithname)
      * [`fn withNamespace(namespace)`](#fn-spectlsoptionswithnamespace)
    * [`obj spec.tls.store`](#obj-spectlsstore)
      * [`fn withName(name)`](#fn-spectlsstorewithname)
      * [`fn withNamespace(namespace)`](#fn-spectlsstorewithnamespace)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of IngressRouteTCP

## obj metadata

"ObjectMeta is metadata that all persisted resources must have, which includes all objects users must create."

### fn metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

### fn metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

**Note:** This function appends passed data to existing values

### fn metadata.withClusterName

```ts
withClusterName(clusterName)
```

"The name of the cluster which the object belongs to. This is used to distinguish resources with same name and namespace in different clusters. This field is not set anywhere right now and apiserver is going to ignore it if set in create or update request."

### fn metadata.withCreationTimestamp

```ts
withCreationTimestamp(creationTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withDeletionGracePeriodSeconds

```ts
withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)
```

"Number of seconds allowed for this object to gracefully terminate before it will be removed from the system. Only set when deletionTimestamp is also set. May only be shortened. Read-only."

### fn metadata.withDeletionTimestamp

```ts
withDeletionTimestamp(deletionTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withFinalizers

```ts
withFinalizers(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

### fn metadata.withFinalizersMixin

```ts
withFinalizersMixin(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

**Note:** This function appends passed data to existing values

### fn metadata.withGenerateName

```ts
withGenerateName(generateName)
```

"GenerateName is an optional prefix, used by the server, to generate a unique name ONLY IF the Name field has not been provided. If this field is used, the name returned to the client will be different than the name passed. This value will also be combined with a unique suffix. The provided value has the same validation rules as the Name field, and may be truncated by the length of the suffix required to make the value unique on the server.\n\nIf this field is specified and the generated name exists, the server will NOT return a 409 - instead, it will either return 201 Created or 500 with Reason ServerTimeout indicating a unique name could not be found in the time allotted, and the client should retry (optionally after the time indicated in the Retry-After header).\n\nApplied only if Name is not specified. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency"

### fn metadata.withGeneration

```ts
withGeneration(generation)
```

"A sequence number representing a specific generation of the desired state. Populated by the system. Read-only."

### fn metadata.withLabels

```ts
withLabels(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

### fn metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

**Note:** This function appends passed data to existing values

### fn metadata.withName

```ts
withName(name)
```

"Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/identifiers#names"

### fn metadata.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the space within which each name must be unique. An empty namespace is equivalent to the \"default\" namespace, but \"default\" is the canonical representation. Not all objects are required to be scoped to a namespace - the value of this field for those objects will be empty.\n\nMust be a DNS_LABEL. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/namespaces"

### fn metadata.withOwnerReferences

```ts
withOwnerReferences(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

### fn metadata.withOwnerReferencesMixin

```ts
withOwnerReferencesMixin(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

**Note:** This function appends passed data to existing values

### fn metadata.withResourceVersion

```ts
withResourceVersion(resourceVersion)
```

"An opaque value that represents the internal version of this object that can be used by clients to determine when objects have changed. May be used for optimistic concurrency, change detection, and the watch operation on a resource or set of resources. Clients must treat these values as opaque and passed unmodified back to the server. They may only be valid for a particular resource or set of resources.\n\nPopulated by the system. Read-only. Value must be treated as opaque by clients and . More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency"

### fn metadata.withSelfLink

```ts
withSelfLink(selfLink)
```

"SelfLink is a URL representing this object. Populated by the system. Read-only.\n\nDEPRECATED Kubernetes will stop propagating this field in 1.20 release and the field is planned to be removed in 1.21 release."

### fn metadata.withUid

```ts
withUid(uid)
```

"UID is the unique in time and space value for this object. It is typically generated by the server on successful creation of a resource and is not allowed to change on PUT operations.\n\nPopulated by the system. Read-only. More info: http://kubernetes.io/docs/user-guide/identifiers#uids"

## obj spec

"IngressRouteTCPSpec defines the desired state of IngressRouteTCP."

### fn spec.withEntryPoints

```ts
withEntryPoints(entryPoints)
```

"EntryPoints defines the list of entry point names to bind to. Entry points have to be configured in the static configuration. More info: https://doc.traefik.io/traefik/v2.9/routing/entrypoints/ Default: all."

### fn spec.withEntryPointsMixin

```ts
withEntryPointsMixin(entryPoints)
```

"EntryPoints defines the list of entry point names to bind to. Entry points have to be configured in the static configuration. More info: https://doc.traefik.io/traefik/v2.9/routing/entrypoints/ Default: all."

**Note:** This function appends passed data to existing values

### fn spec.withRoutes

```ts
withRoutes(routes)
```

"Routes defines the list of routes."

### fn spec.withRoutesMixin

```ts
withRoutesMixin(routes)
```

"Routes defines the list of routes."

**Note:** This function appends passed data to existing values

## obj spec.routes

"Routes defines the list of routes."

### fn spec.routes.withMatch

```ts
withMatch(match)
```

"Match defines the router's rule. More info: https://doc.traefik.io/traefik/v2.9/routing/routers/#rule_1"

### fn spec.routes.withMiddlewares

```ts
withMiddlewares(middlewares)
```

"Middlewares defines the list of references to MiddlewareTCP resources."

### fn spec.routes.withMiddlewaresMixin

```ts
withMiddlewaresMixin(middlewares)
```

"Middlewares defines the list of references to MiddlewareTCP resources."

**Note:** This function appends passed data to existing values

### fn spec.routes.withPriority

```ts
withPriority(priority)
```

"Priority defines the router's priority. More info: https://doc.traefik.io/traefik/v2.9/routing/routers/#priority_1"

### fn spec.routes.withServices

```ts
withServices(services)
```

"Services defines the list of TCP services."

### fn spec.routes.withServicesMixin

```ts
withServicesMixin(services)
```

"Services defines the list of TCP services."

**Note:** This function appends passed data to existing values

## obj spec.routes.middlewares

"Middlewares defines the list of references to MiddlewareTCP resources."

### fn spec.routes.middlewares.withName

```ts
withName(name)
```

"Name defines the name of the referenced Traefik resource."

### fn spec.routes.middlewares.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the namespace of the referenced Traefik resource."

## obj spec.routes.services

"Services defines the list of TCP services."

### fn spec.routes.services.withName

```ts
withName(name)
```

"Name defines the name of the referenced Kubernetes Service."

### fn spec.routes.services.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the namespace of the referenced Kubernetes Service."

### fn spec.routes.services.withPort

```ts
withPort(port)
```

"Port defines the port of a Kubernetes Service. This can be a reference to a named port."

### fn spec.routes.services.withTerminationDelay

```ts
withTerminationDelay(terminationDelay)
```

"TerminationDelay defines the deadline that the proxy sets, after one of its connected peers indicates it has closed the writing capability of its connection, to close the reading capability as well, hence fully terminating the connection. It is a duration in milliseconds, defaulting to 100. A negative value means an infinite deadline (i.e. the reading capability is never closed)."

### fn spec.routes.services.withWeight

```ts
withWeight(weight)
```

"Weight defines the weight used when balancing requests between multiple Kubernetes Service."

## obj spec.routes.services.proxyProtocol

"ProxyProtocol defines the PROXY protocol configuration. More info: https://doc.traefik.io/traefik/v2.9/routing/services/#proxy-protocol"

### fn spec.routes.services.proxyProtocol.withVersion

```ts
withVersion(version)
```

"Version defines the PROXY Protocol version to use."

## obj spec.tls

"TLS defines the TLS configuration on a layer 4 / TCP Route. More info: https://doc.traefik.io/traefik/v2.9/routing/routers/#tls_1"

### fn spec.tls.withCertResolver

```ts
withCertResolver(certResolver)
```

"CertResolver defines the name of the certificate resolver to use. Cert resolvers have to be configured in the static configuration. More info: https://doc.traefik.io/traefik/v2.9/https/acme/#certificate-resolvers"

### fn spec.tls.withDomains

```ts
withDomains(domains)
```

"Domains defines the list of domains that will be used to issue certificates. More info: https://doc.traefik.io/traefik/v2.9/routing/routers/#domains"

### fn spec.tls.withDomainsMixin

```ts
withDomainsMixin(domains)
```

"Domains defines the list of domains that will be used to issue certificates. More info: https://doc.traefik.io/traefik/v2.9/routing/routers/#domains"

**Note:** This function appends passed data to existing values

### fn spec.tls.withPassthrough

```ts
withPassthrough(passthrough)
```

"Passthrough defines whether a TLS router will terminate the TLS connection."

### fn spec.tls.withSecretName

```ts
withSecretName(secretName)
```

"SecretName is the name of the referenced Kubernetes Secret to specify the certificate details."

## obj spec.tls.domains

"Domains defines the list of domains that will be used to issue certificates. More info: https://doc.traefik.io/traefik/v2.9/routing/routers/#domains"

### fn spec.tls.domains.withMain

```ts
withMain(main)
```

"Main defines the main domain name."

### fn spec.tls.domains.withSans

```ts
withSans(sans)
```

"SANs defines the subject alternative domain names."

### fn spec.tls.domains.withSansMixin

```ts
withSansMixin(sans)
```

"SANs defines the subject alternative domain names."

**Note:** This function appends passed data to existing values

## obj spec.tls.options

"Options defines the reference to a TLSOption, that specifies the parameters of the TLS connection. If not defined, the `default` TLSOption is used. More info: https://doc.traefik.io/traefik/v2.9/https/tls/#tls-options"

### fn spec.tls.options.withName

```ts
withName(name)
```

"Name defines the name of the referenced Traefik resource."

### fn spec.tls.options.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the namespace of the referenced Traefik resource."

## obj spec.tls.store

"Store defines the reference to the TLSStore, that will be used to store certificates. Please note that only `default` TLSStore can be used."

### fn spec.tls.store.withName

```ts
withName(name)
```

"Name defines the name of the referenced Traefik resource."

### fn spec.tls.store.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the namespace of the referenced Traefik resource."