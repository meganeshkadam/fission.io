---
title: fission environment update
slug: fission_environment_update
url: /docs/fission-cli/fission_environment_update/
---
## fission environment update

Update an environment

```
fission environment update [flags]
```

### Options

```
      --name string              Environment name
      --image string             Environment image URL
      --poolsize int             Size of the pool (default 3)
      --builder string           Environment builder image URL
      --buildcmd string          Build command for environment builder to build source package
      --imagepullsecret string   Secret for Kubernetes to pull an image from a private registry
      --mincpu int               Minimum CPU to be assigned to pod (In millicore, minimum 1)
      --maxcpu int               Maximum CPU to be assigned to pod (In millicore, minimum 1)
      --minmemory int            Minimum memory to be assigned to pod (In megabyte)
      --maxmemory int            Maximum memory to be assigned to pod (In megabyte)
      --graceperiod int          --period |:|: Grace time (in seconds) for pod to perform connection draining before termination (default value will be used if 0 is given)
      --keeparchive              Keep the archive instead of extracting it into a directory (mainly for the JVM environment because .jar is one kind of zip archive)
      --envNamespace string      --envns |:|: Namespace for environment object (default "default")
      --externalnetwork          Allow pod to access external network (only works when istio feature is enabled)
      --labels string            Comma separated labels to apply to the function. E.g. --labels="environment=dev,application=analytics"
      --annotation stringArray   Annotation to apply to the function. To mention multiple annotations --annotation="abc.com/team=dev" --annotation="foo=bar"
  -h, --help                     help for update
```

### Options inherited from parent commands

```
      --kube-context string   Kubernetes context to be used for the execution of Fission commands
      --server string         Server URL
  -v, --verbosity int         -v |:|: CLI verbosity (0 is quiet, 1 is the default, 2 is verbose) (default 1)
```

### SEE ALSO

* [fission environment](/docs/fission-cli/fission_environment/)	 - Create, update and manage environments

