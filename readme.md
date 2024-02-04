# Awesome Jsonnet [![Awesome](https://awesome.re/badge.svg)][awesome]

> A curated list of [Jsonnet][jsonnet] libraries, utilities, and other resources.

## Contents

- [What is Jsonnet](#what-is-jsonnet)
- [Implementations](#implementations)
- [General](#general)
- [Mixins](#mixins)
- [Kubernetes](#kubernetes)
- [Contribute](#contribute)
- [License](#license)

## What is Jsonnet

A data templating language for app and tool developers

- Generate config data
- Side-effect free
- Organize, simplify, unify
- Manage sprawling config

A simple extension of JSON

- Open source (Apache 2.0)
- Familiar syntax
- Reformatter, linter
- Editor & IDE integrations
- Formally specified

_Source_: [jsonnet.org][jsonnet]

## Implementations

- [jsonnet][google/jsonnet] - Original C++ implementation of Jsonnet.
- [go-jsonnet][google/go-jsonnet] - An implementation of Jsonnet in pure Go.

## General

### Package Management

- [jsonnet-bundler][jsonnet-bundler/jsonnet-bundler] - The jsonnet-bundler is a package manager for Jsonnet.

### Help & Tutorials

- [Jsonnet Tutorial][jsonnet/tutorial] - Official Jsonnet tutorial.
- [Jsonnet Getting Started][jsonnet/getting-started] - Official Jsonnet getting started guide.
- [Implus Jsonnet Tutorial](https://youtu.be/i5PVp92tAmE) - Jsonnet high-level tutorial.
- [Jsonnet Community][jsonnet/community] - Jsonnet communities.

### References

- [Jsonnet Language Reference][jsonnet/language] - Explains Jsonnet in detail.
- [Jsonnet Standard Library Reference][jsonnet/stdlib] - Describes the functions available in Jsonnet's standard library.
- [Jsonnet Style Guide][databricks/jsonnet-style-guide] - Jsonnet coding style guide by Databricks.

### Bindings

- [Jsonnet Bindings][jsonnet/bindings] - Official and recommended 3rd party bindings.
- [terraform-provider-jsonnet][alxrem/terraform-provider-jsonnet] - Terraform provider for generating JSON documents from Jsonnet.

### Extensions

- [JsonnetUnit][yugui/jsonnetunit] - Unit testing framework for Jsonnet.
- [xtd][xtd] - Extended Jsonnet standard library.

### Tools

- [Jsonnet Tooling][jsonnet/tools] - Official and recommended 3rd party tooling.
- [docsonnet][jsonnet-libs/docsonnet] - Jsonnet docs generator.
- [Jsonnet Docblock Parser][legovaer/jsonnet-docblock-parser] - Parser that extracts docblocks from Jsonnet.
- [vscode-jsonnet][grafana/vscode-jsonnet] - VS Code language support for Jsonnet.
- [vim-jsonnet][google/vim-jsonnet] - Jsonnet filetype plugin for Vim.
- [intellij-jsonnet][databricks/intellij-jsonnet] - Intellij Jsonnet Plugin.

## Mixins

Jsonnet packages/libraries that contain Grafana dashboards, Prometheus recording rules, and/or Prometheus alerts. See the [Prometheus Monitoring Mixins Design Doc](https://docs.google.com/document/d/1A9xvzwqnFVSOZ5fD3blKODXfsat5fg6ZhnKu9LK3lB4/view).

### Mixin Websites

- [monitoring.mixins.dev][monitoring.mixins.dev] - Comprehensive resource for mixins.
- [promtools.dev][promtools.dev] - Generate SLOs for Prometheus with Jsonnet. Implements [SLO libsonnet][metalmatze/slo-libsonnet].

### Mixin Libraries

- [Ceph Mixin][ceph/ceph-mixins] - Prometheus alerts for Ceph.
- [cert-manager Mixin][uneeq-oss/cert-manager-mixin] - Prometheus Mixin for [cert-manager][cert-manager].
- [CockroachDB Mixin][metalmatze/kube-cockroachdb-monitoring] - Monitoring definitions for CockroachDB.
- [Consul Mixin][grafana/consul-mixin] - Reuseable and extensible dashboards and alerts for running Hashicorp's Consul.
- [CoreDNS Mixin][povilasv/coredns-mixin] - Grafana dashboard and Prometheus Alerts to monitor CoreDNS.
- [Cortex Mixin][grafana/cortex-mixin] - Monitoring for [cortex-jsonnet][grafana/cortex-jsonnet].
- [ECS Mixin][voronenko/sa_grafonnet_lib] - Set of panels, metrics, templates to visualize state of your ECS clusters.
- [etcd Mixin][etcd-io/etcd-mixin] - Customizable Prometheus alerts for etcd.
- [Gluster Mixin][gluster/gluster-mixins] - Grafana dashboards and Prometheus alerts for Gluster.
- [grafana-builder][grafana/grafana-builder] - Library for building Grafana dashboards with Jsonnet, following the builder pattern.
- [grafana-dashboards][ncabatoff/grafana-dashboards] - Collection of misc Grafana dashboards created by [ncabatoff][ncabatoff].
- [Grafonnet][grafonnet] - Jsonnet library for generating Grafana dashboard files.
- [Jaeger Mixin][grafana/jaeger-mixin] - Grafana's monitoring definitions for Jaeger.
- [Jaeger Mixin][jaegertracing/jaeger-mixin] - Official Prometheus monitoring mixin for Jaeger.
- [Kube State Metrics Mixin][kubernetes/kube-state-metrics-mixin] - Monitoring definitions for Kube State Metrics.
- [Kubernetes Mixin][kubernetes-monitoring/kubernetes-mixin] - Grafana dashboards and Prometheus alerts for Kubernetes.
- [Memcached Mixin][grafana/memcached-mixin] - Reuseable and extensible dashboards for Memcached.
- [mixin-utils][grafana/mixin-utils] - Grafana Labs' mixin utilities.
- [Node Mixin][prometheus/node-mixin] - Monitoring definitions based on the metrics exported by the Node Exporter.
- [Prometheus Ksonnet Mixin][grafana/prometheus-ksonnet] - A set of extensible configurations for running Prometheus on Kubernetes.
- [Prometheus Mixin][prometheus/prometheus-mixin] - Configurable, reusable, and extensible alerts and dashboards for Prometheus.
- [Sealed Secrets Mixin][bitnami-labs/sealed-secrets] - Dashboards, recording rules, alerts and alert tests for Sealed Secrets.
- [SLO libsonnet][metalmatze/slo-libsonnet] - Generate Prometheus alerting & recording rules and Grafana dashboards for your SLOs.
- [Thanos Mixin][thanos-io/mixin] - Extensible and customizable monitoring definitions for Thanos.

### Mixin Tools

- [mixtool][monitoring-mixins/mixtool] - mixtool is a helper for easily working with jsonnet mixins.
- [Grizzly][grafana/grizzly] - A utility for managing Jsonnet dashboards against the Grafana API.

### Mixin Guides & Talks

- [Everything You Need to Know About Monitoring Mixins][1]
- [Tanka: Declarative Dashboards for Declarative Clusters][2] - Grafanacon 2020 talk by Malcolm Holmes.
  - Repo: [tanka-grafanacon-2020][malcolmholmes/tanka-grafanacon-2020]
- [Managing Grafana Dashboards with grafonnet and git](https://youtu.be/kV3Ua6guynI) - PromCon 2019 talk by Adam Wolfe Gordon.
  - Repo: [grafana-dashboards][adamwg/grafana-dashboards]
- [Using Jsonnet to Package Together Dashboards, Alerts, and Exporters][4] - PromCon 2018 talk by Tom Wilkie.
- [Automating Grafana Dashboards with Jsonnet](https://youtu.be/zmsZq9Pfp1g) - Grafanacon 2018 talk by Julien Pivotto.

### Mixin CI/CD

- [Grafonnet Lib Docker][andrewfarley/grafonnet-lib-dockerhub] - Simple Docker image that has Jsonnet and Grafana's grafonnet lib for CI/CD purposes.
- [grafana-dashboards][adamwg/grafana-dashboards] - Example project containing Github actions to automate dashboard CI/CD.

## Kubernetes

### Kubernetes Libraries

- [blackbox-exporter-jsonnet][brancz/blackbox-exporter-jsonnet] - Jsonnet for basic Kubernetes manifests for the [blackbox-exporter][prometheus/blackbox-exporter].
- [cortex-jsonnet][grafana/cortex-jsonnet] - Jsonnet for deploying Cortex and the related monitoring in Kubernetes.
- [ksonnet-loki][grafana/ksonnet-loki] - Jsonnet for deploying Loki in Kubernetes.
- [ksonnet-promtail][grafana/ksonnet-promtail] - Jsonnet for deploying promtail in Kubernetes.
- [kube-cockroachdb][metalmatze/kube-cockroachdb] - Jsonnet for deploying CockroachDB in Kubernetes.
- [kube-prometheus][prometheus-operator/kube-prometheus] - Jsonnet for deploying Prometheus in Kubernetes.
- [kube-state-metrics][kubernetes/kube-state-metrics] - Jsonnet for deploying Kube State Metrics in Kubernetes.
- [kube-thanos][thanos-io/kube-thanos] - Kubernetes specific configuration for deploying Thanos.
- [kubernetes-grafana][brancz/kubernetes-grafana] - Grafana on Kubernetes with Prometheus.
- [oauth2-proxy][jsonnet-libs/oauth2-proxy] - Jsonnet for deploying bitly's OAuth proxy to Kubernetes.

### Kubernetes Tools

- [Tanka][tanka] - [Grafana][grafana]'s reimplementation of [Ksonnet][ksonnet]. Flexible, reusable and concise configuration for Kubernetes.
- [qbec][qbec] - Tool to configure and create Kubernetes objects on multiple environments by [Splunk][splunk].
- [k8s][jsonnet-libs/k8s] - Code generator for the Jsonnet Kubernetes library.

### Kubernetes Guides & Talks

- [How the Jsonnet-based project Tanka improves Kubernetes usage][3] - FOSDEM 2020 talk by Tom Braack and Malcolm Holmes.

## Other Awesome Lists

- [awesome-jsonnet][metalmatze/awesome-jsonnet] by [Matthias Loibl][metalmatze].
- [awesome-libsonnet][sh0rez/awesome-libsonnet] by [sh0rez][sh0rez].

## Similar Languages

- [CUE](https://cuelang.org/)

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)][cc-zero]

To the extent possible under law, Jacob Colvin has waived all copyright and related or neighboring rights to this work.

<!-- Awesome -->
[awesome]: https://awesome.re
[cc-zero]: https://creativecommons.org/publicdomain/zero/1.0

<!-- Jsonnet Pages -->
[jsonnet]: https://jsonnet.org/
[jsonnet/bindings]: https://jsonnet.org/ref/bindings.html
[jsonnet/community]: https://jsonnet.org/learning/community.html
[jsonnet/getting-started]: https://jsonnet.org/learning/getting_started.html
[jsonnet/language]: https://jsonnet.org/ref/language.html
[jsonnet/stdlib]: https://jsonnet.org/ref/stdlib.html
[jsonnet/tools]: https://jsonnet.org/learning/tools.html
[jsonnet/tutorial]: https://jsonnet.org/learning/tutorial.html
[google/jsonnet]: https://github.com/google/jsonnet
[google/go-jsonnet]: https://github.com/google/go-jsonnet

<!-- Project Repos -->
[adamwg/grafana-dashboards]: https://github.com/adamwg/grafana-dashboards
[alxrem/terraform-provider-jsonnet]: https://github.com/alxrem/terraform-provider-jsonnet
[andrewfarley/grafonnet-lib-dockerhub]: https://github.com/AndrewFarley/grafonnet-lib-dockerhub
[brancz/blackbox-exporter-jsonnet]: https://github.com/brancz/blackbox-exporter-jsonnet
[brancz/kubernetes-grafana]: https://github.com/brancz/kubernetes-grafana
[databricks/intellij-jsonnet]: https://github.com/databricks/intellij-jsonnet
[databricks/jsonnet-style-guide]: https://github.com/databricks/jsonnet-style-guide
[google/vim-jsonnet]: https://github.com/google/vim-jsonnet
[grafana/cortex-jsonnet]: https://github.com/grafana/cortex-jsonnet
[grafana/grafana-builder]: https://github.com/grafana/jsonnet-libs/tree/master/grafana-builder
[grafana/grizzly]: https://github.com/grafana/grizzly
[grafana/ksonnet-loki]: https://github.com/grafana/loki/tree/master/production/ksonnet/loki
[grafana/ksonnet-promtail]: https://github.com/grafana/loki/tree/master/production/ksonnet/promtail
[grafana/mixin-utils]: https://github.com/grafana/jsonnet-libs/tree/master/mixin-utils
[grafana/prometheus-ksonnet]: https://github.com/grafana/jsonnet-libs/tree/master/prometheus-ksonnet
[grafana/vscode-jsonnet]: https://github.com/grafana/vscode-jsonnet
[jaegertracing/jaeger-mixin]: https://github.com/jaegertracing/jaeger/tree/master/monitoring/jaeger-mixin
[jsonnet-bundler/jsonnet-bundler]: https://github.com/jsonnet-bundler/jsonnet-bundler
[jsonnet-libs/docsonnet]: https://github.com/jsonnet-libs/docsonnet
[jsonnet-libs/k8s]: https://github.com/jsonnet-libs/k8s
[jsonnet-libs/oauth2-proxy]: https://github.com/grafana/jsonnet-libs/blob/master/oauth2-proxy
[kubernetes/kube-state-metrics]: https://github.com/kubernetes/kube-state-metrics/tree/master/jsonnet/kube-state-metrics
[legovaer/jsonnet-docblock-parser]: https://github.com/legovaer/jsonnet-docblock-parser
[liamdawson/vscode-jsonnet-language]: https://github.com/liamdawson/vscode-jsonnet-language
[malcolmholmes/tanka-grafanacon-2020]: https://github.com/malcolmholmes/tanka-grafanacon-2020
[metalmatze/kube-cockroachdb]: https://github.com/metalmatze/kube-cockroachdb
[metalmatze/slo-libsonnet]: https://github.com/metalmatze/slo-libsonnet
[monitoring-mixins/mixtool]: https://github.com/monitoring-mixins/mixtool
[ncabatoff/grafana-dashboards]: https://github.com/ncabatoff/grafana-dashboards
[prometheus-operator/kube-prometheus]: https://github.com/prometheus-operator/kube-prometheus
[prometheus/blackbox-exporter]: https://github.com/prometheus/blackbox_exporter
[thanos-io/kube-thanos]: https://github.com/thanos-io/kube-thanos
[voronenko/sa_grafonnet_lib]: https://github.com/Voronenko/sa_grafonnet_lib
[yugui/jsonnetunit]: https://github.com/yugui/jsonnetunit

<!-- Project Repos (from monitoring.mixins.dev) -->
[bitnami-labs/sealed-secrets]: https://github.com/bitnami-labs/sealed-secrets/tree/master/contrib/prometheus-mixin
[ceph/ceph-mixins]: https://github.com/ceph/ceph-mixins
[etcd-io/etcd-mixin]: https://github.com/etcd-io/etcd/tree/master/Documentation/etcd-mixin
[gluster/gluster-mixins]: https://github.com/gluster/gluster-mixins
[grafana/consul-mixin]: https://github.com/grafana/jsonnet-libs/tree/master/consul-mixin
[grafana/cortex-mixin]: https://github.com/grafana/cortex-jsonnet/tree/master/cortex-mixin
[grafana/jaeger-mixin]: https://github.com/grafana/jsonnet-libs/tree/master/jaeger-mixin
[grafana/memcached-mixin]: https://github.com/grafana/jsonnet-libs/blob/master/memcached-mixin
[kubernetes-monitoring/kubernetes-mixin]: https://github.com/kubernetes-monitoring/kubernetes-mixin
[kubernetes/kube-state-metrics-mixin]: https://github.com/kubernetes/kube-state-metrics/tree/master/jsonnet/kube-state-metrics-mixin
[metalmatze/kube-cockroachdb-monitoring]: https://github.com/metalmatze/kube-cockroachdb/tree/master/monitoring
[povilasv/coredns-mixin]: https://github.com/povilasv/coredns-mixin
[prometheus-operator/mixin]: https://github.com/prometheus-operator/prometheus-operator/tree/master/jsonnet/mixin
[prometheus/node-mixin]: https://github.com/prometheus/node_exporter/tree/master/docs/node-mixin
[prometheus/prometheus-mixin]: https://github.com/prometheus/prometheus/tree/master/documentation/prometheus-mixin
[thanos-io/mixin]: https://github.com/thanos-io/thanos/tree/master/mixin
[uneeq-oss/cert-manager-mixin]: https://gitlab.com/uneeq-oss/cert-manager-mixin

<!-- Project Websites -->
[cert-manager]: https://cert-manager.io/
[grafana]: https://grafana.com/
[grafonnet]: https://grafana.github.io/grafonnet-lib/
[ksonnet]: https://ksonnet.io/
[monitoring.mixins.dev]: https://monitoring.mixins.dev/
[promtools.dev]: https://promtools.dev
[qbec]: https://qbec.io/
[splunk]: https://splunk.com/
[tanka]: https://tanka.dev/
[xtd]: https://jsonnet-libs.github.io/xtd/

<!-- Articles -->
[1]: https://grafana.com/blog/2018/09/13/everything-you-need-to-know-about-monitoring-mixins/
[2]: https://grafana.com/go/grafanaconline/tanka-declarative-dashboards-for-declarative-clusters/
[3]: https://grafana.com/blog/2020/03/11/how-the-jsonnet-based-project-tanka-improves-kubernetes-usage/
[4]: https://promcon.io/2018-munich/talks/prometheus-monitoring-mixins/

<!-- User Credits -->
[ncabatoff]: https://github.com/ncabatoff
[metalmatze]: https://github.com/metalmatze
[sh0rez]: https://github.com/sh0rez

<!-- Similar Lists -->
[metalmatze/awesome-jsonnet]: https://github.com/metalmatze/awesome-jsonnet
[sh0rez/awesome-libsonnet]: https://github.com/sh0rez/awesome-libsonnet
