# Typhoon

Notable changes between versions.

## v1.7.7

* Kubernetes v1.7.7
* Use kubernetes-incubator/bootkube v0.7.0
* Update kube-dns to 1.14.5 to fix dnsmasq [vulnerability](https://security.googleblog.com/2017/10/behind-masq-yet-more-dns-and-dhcp.html)
* Calico v2.6.1
* flannel-cni v0.3.0
  * Update flannel CNI config to fix hostPort

#### Digital Ocean

* Run etcd cluster across controller nodes (etcd-member.service)
* Reduce time to bootstrap a cluster
* Remove support for self-hosted etcd

## v1.7.5

* Kubernetes v1.7.5
* Use kubernetes-incubator/bootkube v0.6.2
* Add AWS Terraform module (alpha)
* Add support for Calico networking (bare-metal, Google Cloud, AWS)
* Change networking default from "flannel" to "calico"

#### AWS

* Add `network_mtu` to allow CNI interface MTU customization

#### Bare-Metal

* Add `network_mtu` to allow CNI interface MTU customization
* Remove support for `experimental_self_hosted_etcd`

## v1.7.3

* Kubernetes v1.7.3
* Use kubernete-incubator/bootkube v0.6.1

#### Digital Ocean

* Add cloud firewall rules (requires Terraform v0.10)
* Change nodes tags from strings to DO tags

## v1.7.1

* Kubernetes v1.7.1
* Use kubernete-incubator/bootkube v0.6.0
* Add Bare-Metal Terraform module (stable)
* Add Digital Ocean Terraform module (beta)

#### Google Cloud

* Remove `k8s_domain_name` variable, `cluster_name` + `dns_zone` resolves to controllers
* Rename `dns_base_zone` to `dns_zone`
* Rename `dns_base_zone_name` to `dns_zone_name`

## v1.6.7

* Kubernetes v1.6.7
* Use kubernete-incubator/bootkube v0.5.1

## v1.6.6

* Kubernetes v1.6.6
* Use kubernete-incubator/bootkube v0.4.5
* Disable locksmithd on hosts, in favor of [CLUO](https://github.com/coreos/container-linux-update-operator).

## v1.6.4

* Kubernetes v1.6.4
* Add Google Cloud Terraform module (stable)

## Earlier

Earlier versions, back to v1.3.0, used different designs and mechanisms.
