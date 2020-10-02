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
- [vscode-jsonnet-language][liamdawson/vscode-jsonnet-language] - Replacement for the now defunct Hepito VS Code language support.

## Mixins

Jsonnet packages/libraries that contain Grafana dashboards, Prometheus recording rules, and/or Prometheus alerts.

**Readers should begin by visiting [monitoring.mixins.dev][monitoring.mixins.dev], _the_ comprehensive resource for mixins. This repo only includes links to mixin resources not already found on monitoring.mixins.dev.**

### Websites

- [monitoring.mixins.dev][monitoring.mixins.dev] - Comprehensive resource for mixins.
- [promtools.dev][promtools.dev] - Generate SLOs for Prometheus with Jsonnet. Implements [SLO libsonnet][metalmatze/slo-libsonnet].

### Libraries

- [Grafonnet][grafonnet] - Jsonnet library for generating Grafana dashboard files.
- [ECS Mixin][voronenko/sa_grafonnet_lib] - Set of panels, metrics, templates to visualize state of your ECS clusters.
- [Jaeger Mixin][jaegertracing/jaeger-mixin] - Official Prometheus monitoring mixin for Jaeger.
- [grafana-builder][grafana/grafana-builder] - Library for building Grafana dashboards with Jsonnet, following the builder pattern.
- [mixin-utils][grafana/mixin-utils] - Grafana Labs' mixin utilities.
- [SLO libsonnet][metalmatze/slo-libsonnet] - Generate Prometheus alerting & recording rules and Grafana dashboards for your SLOs.
- [Prometheus Ksonnet Mixin][grafana/prometheus-ksonnet] - A set of extensible configurations for running Prometheus on Kubernetes.
- [grafana-dashboards][ncabatoff/grafana-dashboards] - Collection of misc Grafana dashboards created by [ncabatoff][ncabatoff].

### Tools

- [mixtool][monitoring-mixins/mixtool] - mixtool is a helper for easily working with jsonnet mixins.
- [Grizzly][malcolmholmes/grizzly] - A utility for managing Jsonnet dashboards against the Grafana API.

### Guides & Talks

- [Everything You Need to Know About Monitoring Mixins](https://grafana.com/blog/2018/09/13/everything-you-need-to-know-about-monitoring-mixins/)
- [Tanka: Declarative Dashboards for Declarative Clusters](https://grafana.com/go/grafanaconline/tanka-declarative-dashboards-for-declarative-clusters/) - Grafanacon 2020 talk by Malcolm Holmes. Repo: [tanka-grafanacon-2020][malcolmholmes/tanka-grafanacon-2020]
- [Managing Grafana Dashboards with grafonnet and git](https://youtu.be/kV3Ua6guynI) - PromCon 2019 talk by Adam Wolfe Gordon. Repo: [grafana-dashboards][adamwg/grafana-dashboards]
- [Prometheus Monitoring Mixins](https://youtu.be/GDdnL5R_l-Y) - PromCon 2018 talk by Tom Wilkie.
- [Using Jsonnet to Package Together Dashboards, Alerts and Exporters](https://www.youtube.com/watch?v=b7-DtFfsL6E) - Talk by Tom Wilkie.
- [Automating Grafana Dashboards with Jsonnet](https://youtu.be/zmsZq9Pfp1g) - Grafanacon 2018 talk by Julien Pivotto.

### CI/CD

- [Grafonnet Lib Docker][andrewfarley/grafonnet-lib-dockerhub] - Simple Docker image that has Jsonnet and Grafana's grafonnet lib for CI/CD purposes.
- [grafana-dashboards][adamwg/grafana-dashboards] - Example project containing Github actions to automate dashboard CI/CD.

## Kubernetes

### Libraries

- [cortex-jsonnet][grafana/cortex-jsonnet] - Jsonnet for deploying Cortex and the related monitoring in Kubernetes.
- [kube-thanos][thanos-io/kube-thanos] - Kubernetes specific configuration for deploying Thanos.
- [kubernetes-grafana][brancz/kubernetes-grafana] - Grafana on Kubernetes with Prometheus.
- [ksonnet-loki][grafana/ksonnet-loki] - Jsonnet for deploying Loki in Kubernetes.
- [ksonnet-promtail][grafana/ksonnet-promtail] - Jsonnet for deploying promtail in Kubernetes.
- [kube-prometheus][prometheus-operator/kube-prometheus] - Jsonnet for deploying Prometheus in Kubernetes.
- [blackbox-exporter-jsonnet][brancz/blackbox-exporter-jsonnet] - Jsonnet for basic Kubernetes manifests for the [blackbox-exporter][prometheus/blackbox-exporter].
- [oauth2-proxy][jsonnet-libs/oauth2-proxy] - Jsonnet for deploying bitly's OAuth proxy to Kubernetes.

### Tools

- [Tanka][tanka] - [Grafana][grafana]'s reimplementation of [Ksonnet][ksonnet]. Flexible, reusable and concise configuration for Kubernetes.
- [qbec][qbec] - Tool to configure and create Kubernetes objects on multiple environments by [Splunk][splunk].
- [k8s][jsonnet-libs/k8s] - Code generator for the Jsonnet Kubernetes library.

### Guides & Talks

- [How the Jsonnet-based project Tanka improves Kubernetes usage](https://grafana.com/blog/2020/03/11/how-the-jsonnet-based-project-tanka-improves-kubernetes-usage/) - FOSDEM 2020 talk by Tom Braack and Malcolm Holmes.

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
[jsonnet/getting-started]: https://jsonnet.org/learning/getting_started.html
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
[databricks/jsonnet-style-guide]: https://github.com/databricks/jsonnet-style-guide
[grafana/cortex-jsonnet]: https://github.com/grafana/cortex-jsonnet
[grafana/grafana-builder]: https://github.com/grafana/jsonnet-libs/tree/master/grafana-builder
[grafana/ksonnet-loki]: https://github.com/grafana/loki/tree/master/production/ksonnet/loki
[grafana/ksonnet-promtail]: https://github.com/grafana/loki/tree/master/production/ksonnet/promtail
[grafana/mixin-utils]: https://github.com/grafana/jsonnet-libs/tree/master/mixin-utils
[grafana/prometheus-ksonnet]: https://github.com/grafana/jsonnet-libs/tree/master/prometheus-ksonnet
[jaegertracing/jaeger-mixin]: https://github.com/jaegertracing/jaeger/tree/master/monitoring/jaeger-mixin
[jsonnet-bundler/jsonnet-bundler]: https://github.com/jsonnet-bundler/jsonnet-bundler
[jsonnet-libs/docsonnet]: https://github.com/jsonnet-libs/docsonnet
[jsonnet-libs/k8s]: https://github.com/jsonnet-libs/k8s
[jsonnet-libs/oauth2-proxy]: https://github.com/grafana/jsonnet-libs/blob/master/oauth2-proxy
[legovaer/jsonnet-docblock-parser]: https://github.com/legovaer/jsonnet-docblock-parser
[liamdawson/vscode-jsonnet-language]: https://github.com/liamdawson/vscode-jsonnet-language
[malcolmholmes/grizzly]: https://github.com/malcolmholmes/grizzly
[malcolmholmes/tanka-grafanacon-2020]: https://github.com/malcolmholmes/tanka-grafanacon-2020
[metalmatze/slo-libsonnet]: https://github.com/metalmatze/slo-libsonnet
[monitoring-mixins/mixtool]: https://github.com/monitoring-mixins/mixtool
[ncabatoff/grafana-dashboards]: https://github.com/ncabatoff/grafana-dashboards
[prometheus-operator/kube-prometheus]: https://github.com/prometheus-operator/kube-prometheus
[prometheus/blackbox-exporter]: https://github.com/prometheus/blackbox_exporter
[thanos-io/kube-thanos]: https://github.com/thanos-io/kube-thanos
[voronenko/sa_grafonnet_lib]: https://github.com/Voronenko/sa_grafonnet_lib
[yugui/jsonnetunit]: https://github.com/yugui/jsonnetunit

<!-- Project Repos (on monitoring.mixins.dev) -->
[kubernetes-monitoring/kubernetes-mixin]: https://github.com/kubernetes-monitoring/kubernetes-mixin
[prometheus-operator/mixin]: https://github.com/prometheus-operator/prometheus-operator/tree/master/jsonnet/mixin

<!-- Project Websites -->
[grafana]: https://grafana.com/
[grafonnet]: https://grafana.github.io/grafonnet-lib/
[ksonnet]: https://ksonnet.io/
[monitoring.mixins.dev]: https://monitoring.mixins.dev/
[promtools.dev]: https://promtools.dev
[qbec]: https://qbec.io/
[splunk]: https://splunk.com/
[tanka]: https://tanka.dev/
[xtd]: https://jsonnet-libs.github.io/xtd/

<!-- User Credits -->
[ncabatoff]: https://github.com/ncabatoff

<!-- Similar Lists -->
[metalmatze/awesome-jsonnet]: https://github.com/metalmatze/awesome-jsonnet
[sh0rez/awesome-libsonnet]: https://github.com/sh0rez/awesome-libsonnet
