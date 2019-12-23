###### Tekton Pipeline example

https://github.com/tektoncd/pipeline/blob/master/docs/tutorial.md




**Create a secret**

```
kubectl create secret docker-registry regcred \
                     --docker-server=<your-registry-server> \
                     --docker-username=<your-name> \
                     --docker-password=<your-pword> \
                     --docker-email=<your-email>
```


**Create Service Account**
``` 
apiVersion: v1
kind: ServiceAccount
metadata:
  name: tutorial-service
secrets:
  - name: regcred
  
```

**Apply the yaml for the following**

GIT Resource

Image Resource

Task 

    

