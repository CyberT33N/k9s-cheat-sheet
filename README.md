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

## Install/Update
- Neuste Version hier herunterladen:
  - https://github.com/derailed/k9s/releases

Für unsere Linux Fedora Notebooks z.b.:
-  k9s_Linux_x86_64.tar.gz

Das Archiv entpacken und die k9s Datei nach ~/bin/k9s verschieben und die alte ersetzen.






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





<br><br><br><br>

## Logs

<br><br>

#### Logs not showing in Pod
- You can press 0 or:
```bash
~/.k9s/config.yml
k9s.logger.sinceSeconds=-1
```




