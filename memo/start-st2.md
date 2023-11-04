```
$ docker --version
Docker version 20.10.21, build baeda1f

$ docker-compose --version
Docker Compose version v2.11.1

$ docker-compose up -d
[+] Running 20/20
 ⠿ Network st2-docker_private                  Created 0.0s
 ⠿ Network st2-docker_public                   Created 0.1s
 ⠿ Container st2-docker-rabbitmq-1             Started 0.8s
 ⠿ Container st2-docker-st2makesecrets-1       Started 1.0s
 ⠿ Container st2-docker-mongo-1                Started 1.0s
 ⠿ Container st2-docker-redis-1                Started 0.7s
 ⠿ Container st2-docker-st2api-1               Started 1.2s
 ⠿ Container st2-docker-st2actionrunner-1      Started 1.7s
 ⠿ Container st2-docker-st2garbagecollector-1  Started 2.0s
 ⠿ Container st2-docker-st2auth-1              Started 2.6s
 ⠿ Container st2-docker-st2stream-1            Started 2.3s
 ⠿ Container st2-docker-st2timersengine-1      Started 1.7s
 ⠿ Container st2-docker-st2notifier-1          Started 2.5s
 ⠿ Container st2-docker-st2workflowengine-1    Started 2.2s
 ⠿ Container st2-docker-st2sensorcontainer-1   Started 1.8s
 ⠿ Container st2-docker-st2rulesengine-1       Started 2.5s
 ⠿ Container st2-docker-st2scheduler-1         Started 2.2s
 ⠿ Container st2-docker-st2chatops-1           Started 3.3s
 ⠿ Container st2-docker-st2client-1            Started 3.5s
 ⠿ Container st2-docker-st2web-1               Started 3.6s

$ docker-compose ls
NAME                STATUS              CONFIG FILES
st2-docker          running(16)         /home/nbchk/work/github.com/codequokka/st2-docker/docker-compose.yml

$ docker-compose exec st2client bash                                                                                      
Welcome to StackStorm HA v3.7.0 (Ubuntu 20.04.4 LTS GNU/Linux x86_64)                                                     
 * Documentation: https://docs.stackstorm.com/                                                                            
 * Community: https://stackstorm.com/community-signup                                                                     
 * Forum: https://forum.stackstorm.com/                                                                                   
                                                                                                                          
 Here you can use StackStorm CLI. Examples:                                                                               
   st2 action list --pack=core                                                                                            
   st2 run core.local cmd=date                                                                                            
   st2 run core.local_sudo cmd='apt-get update' --tail                                                                    
   st2 execution list                                                                                                     
                                                                                                                          
                                                                                                                          
root@dde6183242dc:/opt/stackstorm# st2 whoami                                                                             
Currently logged in as "st2admin".                                                                                        
                                                                                                                          
Authentication method: authentication token                                                                               
Authentication token expire time: 2022-11-19T22:51:39Z                                                                    
                                                                                                                          
RBAC:                                                                                                                     
 - Enabled: False                                                                                                         
 - Roles:
```
