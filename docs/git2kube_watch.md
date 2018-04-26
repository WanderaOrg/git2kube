## git2kube watch

Decrypt the value server-side and prints the response

### Synopsis

Decrypt the value server-side and prints the response

```
git2kube watch [flags]
```

### Options

```
  -b, --branch string         branch name to pull (default "master")
  -c, --cache-folder string   destination on filesystem where cache of repository will be stored (default "/tmp/git2kube/data/")
  -m, --configmap string      target namespace for resulting ConfigMap
      --exclude strings       regex that if is a match exclude the file from the upload, example: '*.yaml' or 'folder/*' if you want to match a folder (default [^\..*])
  -g, --git string            git repository address, either http(s) or ssh protocol has to be specified
  -h, --help                  help for watch
      --include strings       regex that if is a match include the file in the upload, example: '*.yaml' or 'folder/*' if you want to match a folder (default [.*])
  -i, --interval int          interval in seconds in which to try refreshing ConfigMap from git (default 10)
  -k, --kubeconfig            if locally stored ~/.kube/config should be used, InCluster config will be used if false (default false)
      --merge-type string     how to merge ConfigMap data whether to also delete missing values or just upsert new (options: delete|upsert) (default "delete")
  -n, --namespace string      target namespace for resulting ConfigMap (default "default")
  -v, --verbose               verbose output
```

### SEE ALSO

* [git2kube](git2kube.md)	 - Git to ConfigMap conversion tool
