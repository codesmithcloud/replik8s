---
seo:
  title: Write beautiful docs with Markdown
  description: Ship fast, flexible, and SEO-optimized documentation with beautiful
    design out of the box. Docus brings together the best of the Nuxt ecosystem.
    Powered by Nuxt UI.
---

::u-page-hero
#title
replik8s

#description
Kubernetes controller for synchronising Kubernetes resources across namespaces.

#links
  :::u-button
  ---
  color: neutral
  size: xl
  to: /getting-started/introduction
  trailing-icon: i-lucide-arrow-right
  color: primary
  ---
  Get started
  :::

  :::u-button
  ---
  color: neutral
  icon: simple-icons-github
  size: xl
  to: https://github.com/codesmithtech/replik8s
  target: _blank
  variant: outline
  ---
  Star on GitHub
  :::
::

::u-page-section
#title
Core functionality

#features
  :::u-page-feature
  ---
  icon: streamline-ultimate:synchronize-arrows-three
  ---
  #title
  Synchronise resources across Namespaces

  #description
  Synchronising resources across namespaces is a very common use case. replik8s can sync to existing namespaces, new namespaces on creation and cleans up orphaned resources when the parent resource in the synchronisation tree is deleted.
  :::

  :::u-page-feature
  ---
  icon: material-symbols:dashboard-customize-rounded
  ---
  #title
  Support for Custom Resources

  #description
  All Kubernetes resources (ConfigMaps, Secrets, NetworkPolicies etc.) are supported. You can also synchronise any Custom Resources that you've defined in your cluster. As long as it has a `kind` and `apiVersion`, replik8s can sync it!
  :::

  :::u-page-feature
  ---
  icon: carbon:document-configuration
  ---
  #title
  CRD driven configuration

  #description
  Other replication controllers are driven by annotations - there are several drawbacks to this approach. replik8s uses resources of kind `cloud.codesmith.replik8s/SyncResource` to determine what resources should be synchronised.
  :::
::
