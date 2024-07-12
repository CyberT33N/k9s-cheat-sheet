# K9S Cheat Sheet
K9S Cheat Sheet with the most needed stuff..

<br><br>



Get Pod description
- Press **D**

<br> <br>

Get App Logs
- Press **Enter** on Pod. Then press **Enter** on the App or press **L**








# k9s


<br><br>
<br><br>

## Install/Update
- Neuste Version hier herunterladen:
  - https://github.com/derailed/k9s/releases

You can verify your architecture:
```shell
lscpu
```
- x86_64 = amd64
- https://github.com/derailed/k9s/releases/download/v0.32.5/k9s_linux_amd64.deb








<br><br>

## start with namespace
```bash
k9s -n namespaceNameHere
```



<br><br>

## statefulset
```bash
k9s
:sts
```

<br><br>

## secrets
```bash
k9s
:secrets
```

<br><br>
<br><br>



## Deploy

<br><br>

#### See current deployments
```bash
k9s
:deploy
```

#### Restart deployment
```bash
k9s
:deploy

# Now choose your deployment and press s. Now you can set the replica to 0 and it will shutdown. Then after this set it again to the amount of replicas which it has before. Then it will restart.
```






















<br><br>
<br><br>
________________________________________
________________________________________
<br><br>
<br><br>

# Events
- Use `:events`
- Usefully for debugging if something wents wrong and the container logs are not helping



















<br><br>
<br><br>
________________________________________
________________________________________
<br><br>
<br><br>

## Logs

<br><br>

#### Logs not showing in Pod
- You can press 0 or:
```bash
~/.k9s/config.yml
k9s.logger.sinceSeconds=-1

# Increase terminal buffer size
buffer=100000
```




