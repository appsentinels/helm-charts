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
helm install appsentinels-server appsentinels/appsentinels-server-chart --version 1.3.0
```

## Internal - How publish charts to this repo
```sh
Copy helm package here (get it from helm package <chart dir>
Update index > helm repo index . --url https://appsentinels.github.io/helm-charts --merge index.yaml
git add <helm package>
git add index.yaml
git commit -m "msg"
git push
```
