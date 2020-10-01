# Awesome Jsonnet [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of [Jsonnet](https://jsonnet.org/) libraries, utilities, and other resources.

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

_Source_: [jsonnet.org](https://jsonnet.org/)

## Implementations

- [jsonnet](https://github.com/google/jsonnet) - Original C++ implementation of Jsonnet.
- [go-jsonnet](https://github.com/google/go-jsonnet) - An implementation of Jsonnet in pure Go.

## General

### Package Management

- [jsonnet-bundler](https://github.com/jsonnet-bundler/jsonnet-bundler) - The jsonnet-bundler is a package manager for Jsonnet.

### Guides & Talks

- [Jsonnet Tutorial](https://jsonnet.org/learning/tutorial.html) - Official Jsonnet tutorial.
- [Jsonnet Getting Started](https://jsonnet.org/learning/getting_started.html) - Official Jsonnet getting started guide.
- [Implus Jsonnet Tutorial](https://youtu.be/i5PVp92tAmE) - Jsonnet high-level tutorial.
- [Databricks Jsonnet Guide](https://github.com/databricks/jsonnet-style-guide) - Databricks' Jsonnet coding style guide.

### Extensions

- [JsonnetUnit](https://github.com/yugui/jsonnetunit) - Unit testing framework for Jsonnet.
- [xtd](https://jsonnet-libs.github.io/xtd/) - Extended Jsonnet standard library.

### Tooling

- [Jsonnet Tooling](https://jsonnet.org/learning/tools.html) - Official and recommended 3rd party tooling.
- [vscode-jsonnet-language](https://github.com/liamdawson/vscode-jsonnet-language) - Replacement for the now defunct Hepito VS Code language support.

## Mixins

Jsonnet packages/libraries that contain Grafana dashboards, Prometheus recording rules, and/or Prometheus alerts.

**Readers should begin by visiting [monitoring.mixins.dev](https://monitoring.mixins.dev/), _the_ comprehensive resource for mixins. This repo only includes links to mixin resources not already found on monitoring.mixins.dev.**

### Websites

- [monitoring.mixins.dev](https://monitoring.mixins.dev/) - Comprehensive resource for mixins.
- [promtools.dev](https://promtools.dev) - Generate SLOs for Prometheus with Jsonnet. Implements [SLO libsonnet](https://github.com/metalmatze/slo-libsonnet).

### Libraries

- [Grafonnet](https://grafana.github.io/grafonnet-lib/) - Jsonnet library for generating Grafana dashboard files.
- [ECS Mixin](https://github.com/Voronenko/sa_grafonnet_lib) - Set of panels, metrics, templates to visualize state of your ECS clusters.
- [Jaeger Mixin](https://github.com/jaegertracing/jaeger/tree/master/monitoring/jaeger-mixin) - Official Prometheus monitoring mixin for Jaeger.
- [grafana-builder](https://github.com/grafana/jsonnet-libs/tree/master/grafana-builder) - Library for building Grafana dashboards with Jsonnet, following the builder pattern.
- [mixin-utils](https://github.com/grafana/jsonnet-libs/tree/master/mixin-utils) - Grafana Labs' mixin utilities.
- [SLO libsonnet](https://github.com/metalmatze/slo-libsonnet) - Generate Prometheus alerting & recording rules and Grafana dashboards for your SLOs.
- [grafana-dashboards](https://github.com/ncabatoff/grafana-dashboards) - Collection of Grafana dashboards created by [ncabatoff](https://github.com/ncabatoff).

### Tools

- [mixtool](https://github.com/monitoring-mixins/mixtool) - mixtool is a helper for easily working with jsonnet mixins.
- [Grizzly](https://github.com/malcolmholmes/grizzly) - A utility for managing Jsonnet dashboards against the Grafana API.

### Guides & Talks

- [Everything You Need to Know About Monitoring Mixins](https://grafana.com/blog/2018/09/13/everything-you-need-to-know-about-monitoring-mixins/)
- [Tanka: Declarative Dashboards for Declarative Clusters](https://grafana.com/go/grafanaconline/tanka-declarative-dashboards-for-declarative-clusters/) - Grafanacon 2020 talk by Malcolm Holmes. Repo: [tanka-grafanacon-2020](https://github.com/malcolmholmes/tanka-grafanacon-2020)
- [Managing Grafana Dashboards with grafonnet and git](https://youtu.be/kV3Ua6guynI) - PromCon 2019 talk by Adam Wolfe Gordon. Repo: [grafana-dashboards](https://github.com/adamwg/grafana-dashboards)
- [Prometheus Monitoring Mixins](https://youtu.be/GDdnL5R_l-Y) - PromCon 2018 talk by Tom Wilkie.
- [Using Jsonnet to Package Together Dashboards, Alerts and Exporters](https://www.youtube.com/watch?v=b7-DtFfsL6E) - Talk by Tom Wilkie.
- [Automating Grafana Dashboards with Jsonnet](https://youtu.be/zmsZq9Pfp1g) - Grafanacon 2018 talk by Julien Pivotto.

### CI/CD

- [Grafonnet Lib Docker](https://github.com/AndrewFarley/grafonnet-lib-dockerhub) - A simple Docker image that has Jsonnet and Grafana's grafonnet lib for CI/CD purposes.
- [grafana-dashboards](https://github.com/adamwg/grafana-dashboards) - An example project containing Github actions to automate dashboard CI/CD.

## Kubernetes

### Libraries

- [cortex-jsonnet](https://github.com/grafana/cortex-jsonnet) - Jsonnet for deploying Cortex and the related monitoring in Kubernetes.
- [kube-thanos](https://github.com/thanos-io/kube-thanos) - Kubernetes specific configuration for deploying Thanos.
- [kubernetes-grafana](https://github.com/brancz/kubernetes-grafana) - The future of Grafana on Kubernetes with Prometheus.
- [prometheus-operator](https://github.com/coreos/prometheus-operator/tree/master/jsonnet/prometheus-operator) - Jsonnet for deploying Prometheus Operator in Kubernetes.
- [kube-prometheus](https://github.com/coreos/kube-prometheus/tree/master/jsonnet/kube-prometheus) - Jsonnet for deploying Prometheus in Kubernetes.
- [blackbox-exporter-jsonnet](https://github.com/brancz/blackbox-exporter-jsonnet) - Jsonnet code for basic Kubernetes manifests for the [blackbox-exporter](https://github.com/prometheus/blackbox_exporter).

### Tools

- [Tanka](https://tanka.dev/) - Flexible, reusable and concise configuration for Kubernetes by [Grafana](https://grafana.com/).
- [qbec](https://qbec.io/) - A tool to configure and create Kubernetes objects on multiple environments by [Splunk](https://www.splunk.com/).

### Guides & Talks

- [How the Jsonnet-based project Tanka improves Kubernetes usage](https://grafana.com/blog/2020/03/11/how-the-jsonnet-based-project-tanka-improves-kubernetes-usage/) - FOSDEM 2020 talk by Tom Braack and Malcolm Holmes.

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, Jacob Colvin has waived all copyright and related or neighboring rights to this work.
