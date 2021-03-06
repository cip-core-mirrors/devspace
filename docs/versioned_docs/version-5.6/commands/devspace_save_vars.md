---
title: "Command - devspace save vars"
sidebar_label: devspace save vars
---


Saves variable values to kubernetes

## Synopsis


```
devspace save vars [flags]
```

```
#######################################################
################ devspace save vars ###################
#######################################################
Saves devspace config variable values into a kubernetes 
secret. Variable values can be shared or restored via
devspace restore vars.

Examples:
devspace save vars
devspace save vars --namespace test 
devspace save vars --vars-secret my-secret
#######################################################
```


## Flags

```
  -h, --help                 help for vars
      --vars-secret string   The secret to use to save the variables into (default "devspace-vars")
```


## Global & Inherited Flags

```
      --config string         The devspace config file to use
      --debug                 Prints the stack trace if an error occurs
      --kube-context string   The kubernetes context to use
  -n, --namespace string      The kubernetes namespace to use
      --no-warn               If true does not show any warning when deploying into a different namespace or kube-context than before
  -p, --profile string        The devspace profile to use (if there is any)
      --profile-refresh       If true will pull and re-download profile parent sources
      --silent                Run in silent mode and prevents any devspace log output except panics & fatals
  -s, --switch-context        Switches and uses the last kube context and namespace that was used to deploy the DevSpace project
      --var strings           Variables to override during execution (e.g. --var=MYVAR=MYVALUE)
```

