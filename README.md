# AppSentinels helm charts

## Add the Helm repo
```sh
helm repo add appsentinels https://appsentinels.github.io/helm-charts
helm repo update
```

## Search for available charts
```sh
helm search repo appsentinels
```

## Install a chart
```sh
helm install my-edge appsentinels/edge-controller --version <version>
helm install my-sniffer appsentinels/sniffer --version <version>
helm install my-dast-client appsentinels/dastclient --version 1.0.0
```
