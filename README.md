![router setup](https://user-images.githubusercontent.com/83507970/170120644-be13ee8c-486c-43e5-a2ce-f88c4f2aaaa5.png)

# Script for install Connext Router `0.2.0-beta.0`



### Requirements

- OS Ubuntu 18.04 or 20.04 
- Need Super user or root for run this script.
- You can check the current Router version in the https://github.com/connext/nxtp/releases


## Clone and Install Scripts

```

wget -q -O nxtp-router-pk.sh https://raw.githubusercontent.com/NunoyHaxxana/nxtp-router-docker-config/main/nxtp-router-pk.sh && chmod +x nxtp-router-pk.sh && sudo /bin/bash nxtp-router-pk.sh
```




![image](https://user-images.githubusercontent.com/83507970/170120882-96064529-8c8f-444d-880a-c9f4e188f6b1.png)

Choose you wanted option (for example option 1 Install with Auto PKey), press enter and wait for installation to complete.

 1) Install with Auto PKey
> Install router and auto gen private key on key.yaml

 2) Install with Your PKey
> Install router with your private key

 3) Upgrade Version
> Upgrade router to new version

 4) Backup PKey
> Backup and show your private key

 5) Delete
> Delete Router and Data File












### (Optional) Command
- Monitor router real time log.
```
docker logs --follow --tail 100 router
```


- Check the status.
```
docker-compose ps 
OR 
docker ps -a
```

- Restart Docker
```
docker-compose restart
```

- Stop and delete containers.

```
docker-compose down
```




