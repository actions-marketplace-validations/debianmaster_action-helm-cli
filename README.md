
# Publish helm 3 chart
Publish helm3 chart to charts museum.

```yaml
    - uses: actions/checkout@v2
    - uses: debianmaster/action-helm-cli@master
      env:
        SOURCE_DIR: 'charts'
        CHART_FOLDER: 'test-chart'
        FORCE: 'True'
        CHARTMUSEUM_URL: 'https://charts.example.sh'
        CHARTMUSEUM_USER: '${{ secrets.CHARTMUSEUM_USER }}'
        CHARTMUSEUM_PASSWORD: ${{ secrets.CHARTMUSEUM_PASSWORD }}
```
