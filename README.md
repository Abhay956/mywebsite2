
# example of CI/CD of OpenShift
![image](https://github.com/Abhay956/mywebsite2/assets/132220412/a3bcfebe-f91b-47e3-892a-7cd1b7445cd7)


first deploy web-app with these commands


## commands

To deploy this project run

```bash
oc new-app --name=myweb https://github.com/Abhay956/mywebsite2.git
```
check pod is runing or not if it is running, then create route.
 ```bash
oc get pod
oc get svc
oc expose svc myweb
```
then copy route host port and past in brower.
output look like this....
![image](https://github.com/Abhay956/mywebsite2/assets/132220412/f2202599-18c8-439b-be5c-7b8a68c1e601)

#### now time to change code change background image link and text of this is version1 change as version2 then apply this command.
 ```bash
oc start-build myweb
```
now output is change.

![image](https://github.com/Abhay956/mywebsite2/assets/132220412/9baccf3d-739d-4fbb-bd8c-89926ad98c28)

this is first wallpaper link:- https://wallpapers.com/images/hd/coniferous-forest-lake-bub7kqwrdxapq1t8.webp 

this is second wallpaper link:- https://wallpapers.com/images/hd/lush-green-forest-neblzag5t76yolal.webp
