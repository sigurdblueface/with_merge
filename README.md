# with_merge
[issue #1756](https://github.com/roboll/helmfile/issues/1756)
## steps to reproduce
```
docker run -it -v $(pwd):/test quay.io/roboll/helmfile:helm3-v0.130.1 sh -c "cd test; helmfile template > template-0.130.1" 
docker run -it -v $(pwd):/test quay.io/roboll/helmfile:helm3-v0.130.2 sh -c "cd test; helmfile template > template-0.130.2"
```