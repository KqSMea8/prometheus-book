# 目录

* [全书组织](Introduction.md)

## Part I - Prometheus基础

* [第1章 天降奇兵](./quickstart/README.md)
  * [Prometheus简介](./quickstart/why-monitor.md)
  * [初识Prometheus](./quickstart/prometheus-quick-start.md)
    * [安装Prometheus Server](./quickstart/install-prometheus-server.md)
    * [使用Node Exporter采集主机数据](./quickstart/use-node-exporter.md)
    * [使用PromQL查询监控数据](./quickstart/promql_quickstart.md)
    * [监控数据可视化](./quickstart/use-grafana-create-dashboard.md)
  * [任务和实例](./quickstart/prometheus-job-and-instance.md)
  * [Prometheus核心组件](./quickstart/prometheus-architecture-and-components.md)
  * 对比其它监控解决方案
  * [小结](./quickstart/SUMMARY.md)
* [第2章 探索PromQL](./promql/README.md)
  * [理解时间序列](./promql/what-is-prometheus-metrics-and-labels.md)
  * [Metrics类型](./promql/prometheus-metrics-types.md)
    * Counter计数器
    * Gauges仪表盘
    * Histograms桶
    * Summaries概要
  * [初识PromQL](./promql/prometheus-query-language.md)
  * [PromQL操作符](./promql/prometheus-promql-operators-v2.md)
  * [PromQL聚合操作](./promql/prometheus-aggr-ops.md)
  * [PromQL内置函数](./promql/prometheus-promql-functions.md)
  * [在HTTP API中使用PromQL](./promql/prometheus-promql-with-http-api.md)
  * [最佳实践：4个黄金指标和USE方法](./promql/prometheus-promql-best-praticase.md)
  * [小结](./promql/SUMMARY.md)
* [第3章 Prometheus告警处理](./alert/README.md)
  * [Prometheus告警简介](./alert/prometheus-alert-manager-overview.md)
  * [自定义Prometheus告警规则](./alert/prometheus-alert-rule.md)
  * [部署AlertManager](./alert/install-alert-manager.md)
  * [基于Label的动态告警处理](./alert/alert-manager-routes.md)
  * [内置告警接收器Receiver](./alert/alert-manager-with-smtp.md)
    * 集成邮件系统
    * 集成Slack
    * 集成微信
    * 使用Webhook
      * 集成企业钉钉
    * 告警模板详解
  * [使用Webhook扩展Alertmanager](./alert/alert-manager-extension-with-webhook.md)
  * [屏蔽告警通知](./alert/alert-manager-inhibit.md)
  * [使用Recoding Rules优化性能](./alert/prometheus-recoding-rules.md)
  * [小结](./alert/SUMMARY.md)

## Part II - Prometheus进阶

* [第4章 Exporter详解](./exporter/README.md)
  * [Exporter是什么](./exporter/what-is-prometheus-exporter.md)
  * [常用Exporter](./exporter/commonly-eporter-usage.md)
    * [容器监控：cAdvisor](./exporter/use-prometheus-monitor-container.md)
    * [监控MySQL运行状态：MySQLD Exporter](./exporter/use-promethues-monitor-mysql.md)
    * [网络探测：Blackbox Exporter](./exporter/install_blackbox_exporter.md)
  * [使用Java自定义Exporter](./exporter/custom_exporter_with_java.md)
    * [使用client_java](./exporter/client_library_java.md)
    * [在Spring Boot中集成](./exporter/custom_app_support_prometheus.md)
  * [小结](./exporter/SUMMARY.md)
* [第5章 数据与可视化](./grafana/README.md)
  * [使用Console Template](./grafana/console-template)
  * [Grafana详解](./grafana/grafana-intro.md)
    * [使用Panel可视化监控数据](./grafana/grafana-panels.md)
      * [变化趋势：Graph面板](./grafana/use_graph_panel.md)
      * [分布统计：Heatmap面板](./grafana/use_heatmap_panel.md)
      * [当前状态：SingleStat面板](./grafana/use_singlestat_panel.md)
      * [表格：Tabel面板](./grafana/use_table_panel.md)
    * [模板化Dashboard](./grafana/templating.md)
    * [共享Dashboard](./grafana/share_dashboard.md)
  * [小结](./grafana/SUMMARY.md)
* [第6章 集群与高可用](./ha/READMD.md)
  * [本地存储](./ha/prometheus-local-storage.md)
  * [远程存储](./ha/prometheus-remote-storage.md)
  * [联邦集群](./ha/scale-prometheus-with-federation.md)
  * [Prometheus高可用](./ha/prometheus-and-high-availability.md)
  * [Alertmanager高可用](./ha/alertmanager-high-availability.md)
  * [总结](./ha/SUMMARY.md)
* [第7章 Prometheus服务发现](./sd/README.md)
  * [Prometheus与服务发现](./sd/why-need-service-discovery.md)
  * [基于文件的服务发现](./sd/service-discovery-with-file.md)
  * [基于Consul的服务发现](./sd/service-discovery-with-consul.md)
  * 自定义服务发现
  * [服务发现与Relabel](./sd/service-discovery-with-relabel.md)
  * [小结](./sd/SUMMARY.md)

## Part III - Prometheus实战

* [第8章 监控Kubernetes](./kubernetes/READMD.md)
  * [初识Kubernetes](./kubernetes/kubernetes-with-minikube.md)
  * [部署Prometheus](./kubernetes/deploy-prometheus-in-kubernetes.md)
  * [Kubernetes下的服务发现](./kubernetes/service-discovery-with-kubernetes.md)
  * [监控Kubernetes集群](./kubernetes/use-prometheus-monitor-kubernetes.md)
  * [使用Grafana创建可视化仪表盘](./kubernetes/use-grafana-in-k8s.md)
  * [基于Prometheus的弹性伸缩](./kubernetes/hap-with-prometheus.md)
  * [小结](./kubernetes/SUMMARY.md)
* 第9章 Prometheus Operator
  * [使用Opertor管理Prometheus](./kubernetes/use-operator-manage-prometheus.md)
  * [使用Prometheus Operator监控用户应用](./kubernetes/use-operator-monitor-app.md)
  * [使用Prometheus Operator管理Alertmanager](./kubernetes/use-operator-alerting.md)
* [第10章 使用Prometheus监控Rancher集群](./rancher/README.md)
* [参考资料](./REFERENCES.md)
