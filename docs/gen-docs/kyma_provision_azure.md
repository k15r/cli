## kyma provision azure

Provisions an Azure Kubernetes Service (AKS) cluster on Azure.

### Synopsis

Use this command to provision a Kubernetes cluster on Azure for Kyma installation. Use the flags to specify cluster details.
NOTE: To provision and access the provisioned cluster, make sure you get authenticated by using the Azure CLI. To do so,run `az login` and log in with your Azure credentials.

```
kyma provision azure [flags]
```

### Options

```
  -c, --credentials string    Path to the TOML file containing the Azure Client ID (CLIENT_ID) and Client Secret (CLIENT_SECRET). (required)
      --disk-size int         Disk size (in GB) of the cluster. (default 35)
  -k, --kube-version string   Kubernetes version of the cluster. (default "1.15")
  -l, --location string       Location of the cluster. (default "westeurope")
  -n, --name string           Name of the Azure cluster to provision. (required)
      --nodes int             Number of cluster nodes. (default 3)
  -p, --project string        Name of the Azure Resource Group where you provision the Azure cluster. (required)
  -t, --type string           Machine type used for the cluster. (default "Standard_D2_v3")
```

### Options inherited from parent commands

```
      --ci                  Enables the CI mode to run on CI/CD systems.
  -h, --help                Displays help for the command.
      --kubeconfig string   Specifies the path to the kubeconfig file. By default, Kyma CLI uses the KUBECONFIG environment variable or "/$HOME/.kube/config" if the variable is not set.
      --non-interactive     Enables the non-interactive shell mode.
  -v, --verbose             Displays details of actions triggered by the command.
```

### SEE ALSO

* [kyma provision](kyma_provision.md)	 - Provisions a cluster for Kyma installation.

###### Auto generated by spf13/cobra on 23-Apr-2020
