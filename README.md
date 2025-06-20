# Fredx30 Helm Charts

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

    helm repo add fredx30 https://charts.dyrvold.dev/

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
bitwarden` to see the charts.

We recommend creating a namespace for the self-host deployment.

To install/upgrade the self-host chart:

    helm upgrade emby fredx30/emby --install --namespace media --values values.yaml

To uninstall the chart:

    helm uninstall emby --namespace media