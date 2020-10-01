# Awesome Jsonnet [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of [Jsonnet](https://jsonnet.org/) libraries, utilities, and other resources.

## Contents

- [Legend](#legend)
- [What is Jsonnet](#what-is-jsonnet)
- [Implementations](#implementations)
- [General](#general)
- [Mixins](#mixins)
- [Kubernetes](#kubernetes)
- [Contribute](#contribute)
- [License](#license)

## Legend

- Abandoned / Outdated :skull:
- Alpha / WIP :construction:

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
- [Jsonnet](https://youtu.be/i5PVp92tAmE) - Jsonnet high-level tutorial.
- [Databricks Jsonnet Guide](https://github.com/databricks/jsonnet-style-guide) - Databricks' Jsonnet coding style guide.

### Extensions

- [JsonnetUnit](https://github.com/yugui/jsonnetunit) - Unit testing framework for Jsonnet.
- [xtd](https://jsonnet-libs.github.io/xtd/) - Extended Jsonnet standard library.

### Tooling

- [Jsonnet Tooling](https://jsonnet.org/learning/tools.html) - Official and recommended 3rd party tooling.
- [vscode-jsonnet-language](https://github.com/liamdawson/vscode-jsonnet-language) - Replacement for the now defunct Hepito vscode language support.

## Mixins

Jsonnet packages/libraries that contain Grafana dashboards, Prometheus recording rules, and/or Prometheus alerts.

### Websites

- [monitoring.mixins.dev](https://monitoring.mixins.dev/) - Comprehensive resource for mixins.
- [promtools.dev](https://promtools.dev) - Generate SLOs for Prometheus with Jsonnet. Implements [SLO libsonnet](https://github.com/metalmatze/slo-libsonnet).

### Libraries

- [Grafonnet](https://grafana.github.io/grafonnet-lib/) - Jsonnet library for generating Grafana dashboard files.
- [Prometheus Mixin](https://github.com/prometheus/prometheus/tree/master/documentation/prometheus-mixin) :construction: - Set of Jsonnet alerts and dashboards for Prometheus.
- [ECS Mixin](https://github.com/Voronenko/sa_grafonnet_lib) - Set of panels, metrics, templates to visualize state of your ECS clusters.
- [Jaeger Mixin](https://github.com/jaegertracing/jaeger/tree/master/monitoring/jaeger-mixin) - Prometheus monitoring mixin for Jaeger.
- [Kubernetes Mixin](https://github.com/kubernetes-monitoring/kubernetes-mixin) :construction: - A set of Grafana dashboards and Prometheus alerts for Kubernetes.
- [Cortex Mixin](https://github.com/grafana/cortex-jsonnet) - This repo has the jsonnet for deploying cortex and the related monitoring in Kubernetes.
- [Thanos Mixin](https://github.com/thanos-io/thanos/tree/master/mixin) :construction: - This directory contains extensible and customizable monitoring definitions for Thanos.
- [grafana-builder](https://github.com/grafana/jsonnet-libs/tree/master/grafana-builder) - A library for building Grafana dashboards with jsonnet, following the builder pattern.
- [mixin-utils](https://github.com/grafana/jsonnet-libs/tree/master/mixin-utils) - Grafana Labs' mixin utilities.
- [Prometheus Ksonnet Mixin](https://github.com/grafana/jsonnet-libs/tree/master/prometheus-ksonnet) :skull: - A set of extensible configurations for running Prometheus on Kubernetes.
- [HashiCorp Consul Mixin](https://github.com/grafana/jsonnet-libs/tree/master/consul-mixin) - A set of reuseable and extensible dashboards and alerts for running Hashicorp's Consul.
- [Memcached Mixin](https://github.com/grafana/jsonnet-libs/blob/master/memcached-mixin) - A set of reuseable and extensible dashboards for Memcached.
- [SLO libsonnet](https://github.com/metalmatze/slo-libsonnet) :construction: - Generate Prometheus alerting & recording rules and Grafana dashboards for your SLOs.
- [ksonnet-lib](https://github.com/ksonnet/ksonnet-lib) :skull: - Generated mixins for Kubernetes used by ksonnet.

### Tools

- [mixtool](https://github.com/monitoring-mixins/mixtool) :construction: - mixtool is a helper for easily working with jsonnet mixins.
- [Grizzly](https://github.com/malcolmholmes/grizzly) :construction: - A utility for managing Jsonnet dashboards against the Grafana API.

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

- [cortex-jsonnet](https://github.com/grafana/cortex-jsonnet) - This repo has the jsonnet for deploying cortex and the related monitoring in Kubernetes.
- [kube-thanos](https://github.com/thanos-io/kube-thanos) - Kubernetes specific configuration for deploying Thanos.
- [kubernetes-grafana](https://github.com/brancz/kubernetes-grafana) - The future of Grafana on Kubernetes with Prometheus.
- [prometheus-operator](https://github.com/coreos/prometheus-operator/tree/master/jsonnet/prometheus-operator) - This repo has the jsonnet for deploying Prometheus Operator in Kubernetes.
- [ksonnet-loki](https://github.com/grafana/loki/tree/master/production/ksonnet/loki) :skull: - This repo has the jsonnet for deploying Loki in Kubernetes.
- [ksonnet-promtail](https://github.com/grafana/loki/tree/master/production/ksonnet/promtail) :skull: - This repo has the jsonnet for deploying promtail in Kubernetes.
- [kube-prometheus](https://github.com/coreos/kube-prometheus/tree/master/jsonnet/kube-prometheus) - This repo has the jsonnet for deploying Prometheus in Kubernetes.
- [ksonnet-util](https://github.com/grafana/jsonnet-libs/blob/master/ksonnet-util) :skull: - An overlay and set of utilities for ksonnet that makes working with the library easier.
- [oauth2-proxy](https://github.com/grafana/jsonnet-libs/blob/master/oauth2-proxy) - A ksonnet configuration for deploying bitly's OAuth proxy to Kubernetes.

### Tools

- [Tanka](https://tanka.dev/) - Flexible, reusable and concise configuration for Kubernetes by [Grafana](https://grafana.com/).
- [qbec](https://qbec.io/) - A tool to configure and create Kubernetes objects on multiple environments by [Splunk](https://www.splunk.com/).
- [ksonnet](https://ksonnet.io) :skull: - Streamline how you write and deploy Kubernetes configurations by [Heptio](https://heptio.com) & [bitnami](https://bitnami.com).

### Guides & Talks

- [How the Jsonnet-based project Tanka improves Kubernetes usage](https://grafana.com/blog/2020/03/11/how-the-jsonnet-based-project-tanka-improves-kubernetes-usage/) - FOSDEM 2020 talk by Tom Braack and Malcolm Holmes.
- [YAML is for Computers. ksonnet is for Humans](https://www.youtube.com/watch?v=FjdS21McgpE) :skull: - Talk by Bryan Liles, Heptio (Any Skill Level).

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, Jacob Colvin has waived all copyright and related or neighboring rights to this work.