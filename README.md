### Overview 
Kali ini saya akan membuat sebuah case page dimana saya akan mengotak otak sebuah infrastructure yang sudah saya buat sebelumnya,nah kali ini saya 
akan mengotak atik infra dari pull based yang sudah saya buat dan sedikit mengubahnya,jika di projek utama infra pull based semua cluster memiliki 
satu argocd bisa di sebut bahwa infra itu stand alone argocd nah tapi untuk yang kali ini hanya akan ada satu argocd di dua cluster dan infra ini
disebut dengan hub and spoke infrastructure,dan untuk hub akan di cluster jakarta dan untuk spokenya akan di cluster bandung,oke tidak usah berlama-
lama langsung saja masuk ke pembahasannya

| Node        | CPU     | RAM  | Storage | Network                                             |
|-------------|---------|------|---------|---------------------------------------------------- |
| **Master-cluster-Jakarta**  | 2 cores | 2GB  | 10GB    | 1 Adapters   ( Static Ip )          |
| **Worker 1-cluster-Jakarta**| 2 cores | 2GB  | 10GB    | 1 Adapters   ( Static Ip )          |
| **Worker 2-cluster-Jakarta**| 2 cores | 2GB  | 10GB    | 1 Adapters   ( Static Ip )          |
| **Master-cluster-Bandung**  | 2 cores | 2GB  | 10GB    | 1 Adapters   ( Static Ip )          |
| **Worker 1-cluster-Bandung**| 2 cores | 2GB  | 10GB    | 1 Adapters   ( Static Ip )          |
| **Worker 2-Cluster-Bandung**| 2 cores | 2GB  | 10GB    | 1 Adapters   ( Static Ip )          |
| **Jenkins**                 | 7 cores | 7GB  | 240GB   |                Wlan                 |


![asciadbv](/asset/Neon GitOps Hub-and-Spoke Architecture Workflow.png)


