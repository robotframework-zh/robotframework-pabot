# robotframework-pabot
pabot command in docker environment

![pabot-docker](https://github.com/wywincl/robotframework-pabot/blob/master/pabot-docker.jpg)

`pabot` is parallel executor for Robot Framework test cases. [see more](https://github.com/mkorpela/pabot)


# usage

#### use pabot to run test
```
docker run --rm -v {yourpath}:/etc/robot wywincl/robotframework-pabot [options] testcases  
```

#### use robot to run test 
```
docker run --rm -v {yourpath}:/etc/robot --entrypoint="robot" wywincl/robotframework-pabot [options] testcases  
```

# examples

*scenario 1*

```
docker run --rm -v /testdir:/etc/robot wywincl/robotframework-pabot -d /etc/robot/results testcases  
```
