# charts
Helm charts

## Create a directory of chart and packages
Create a folders on root repository folder
```
mkdir Charts
mkdir Packages
```
## Create a new chart
Access the Chart folder
```
cd Charts
helm create ${chart-name}
```
## Create a package from Chart
Access the root repository folder
```
cd ..
helm package Charts/${chart-name}
```

## Move de package to PAckages
Access the root repository folder
```
mv ${chart-name}-0.1.0.tgz Packages/
```

## Create a index
Access the root repository folder

````
helm repo index .
````

## ADD helm repo
Add helm repo


```
helm repo add demo-app https://${username}.github.io/${repository-name}

```

## List repository
```
helm repo list
```