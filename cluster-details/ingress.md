# Ingress

**Ingress Class Configuration**

Kloudlite Kubernetes clusters are configured to support ingress on standard HTTP and HTTPS ports: 80 and 443. By default, the clusters are equipped with an ingress class labeled `nginx.`

**Ingress Controller Operation**

The Kloudlite ingress controller operates in daemon mode across all nodes within the cluster. This setup ensures dedicated availability of ports 80 and 443 on each node for efficient traffic management.

**CName - DNS record**

Kloudlite simplifies the DNS configuration process. Each cluster is assigned a CName, which is directly mapped to the A records of the cluster's nodes. This feature allows for straightforward domain pointing – users can link their domains to the cluster by referencing the CName provided in the cluster overview.

**TLS Certificate Management**

Kloudlite do certificate management with [cert-manager.io](https://cert-manager.io/). Presently, Kloudlite offers support for managing wildcard TLS certificates through [Cloudflare](https://www.cloudflare.com/). This integration facilitates enhanced security and streamlined certificate handling for your applications.
