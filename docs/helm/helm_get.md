## helm get

download a named release

### Synopsis


This command shows the details of a named release.

It can be used to get extended information about the release, including:

  - The values used to generate the release
  - The chart used to generate the release
  - The generated manifest file

By default, this prints a human readable collection of information about the
chart, the supplied values, and the generated manifest file.


```
helm get [flags] RELEASE_NAME
```

### Options

```
  -h, --help                  help for get
      --revision int32        get the named release with revision
      --template string       go template for formatting the output, eg: {{.Release.Name}}
      --tls                   enable TLS for request
      --tls-ca-cert string    path to TLS CA certificate file (default "$HELM_HOME/ca.pem")
      --tls-cert string       path to TLS certificate file (default "$HELM_HOME/cert.pem")
      --tls-hostname string   the server name used to verify the hostname on the returned certificates from the server
      --tls-key string        path to TLS key file (default "$HELM_HOME/key.pem")
      --tls-verify            enable TLS for request and verify remote
```

### Options inherited from parent commands

```
      --debug                           enable verbose output
      --home string                     location of your Helm config. Overrides $HELM_HOME (default "~/.helm")
      --host string                     address of Tiller. Overrides $HELM_HOST
      --kube-context string             name of the kubeconfig context to use
      --kubeconfig string               absolute path to the kubeconfig file to use
      --tiller-connection-timeout int   the duration (in seconds) Helm will wait to establish a connection to tiller (default 300)
      --tiller-namespace string         namespace of Tiller (default "kube-system")
```

### SEE ALSO

* [helm](helm.md)	 - The Helm package manager for Kubernetes.
* [helm get hooks](helm_get_hooks.md)	 - download all hooks for a named release
* [helm get manifest](helm_get_manifest.md)	 - download the manifest for a named release
* [helm get notes](helm_get_notes.md)	 - displays the notes of the named release
* [helm get values](helm_get_values.md)	 - download the values file for a named release

###### Auto generated by spf13/cobra on 25-Mar-2019
