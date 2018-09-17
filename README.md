# Bounce-port-8080

### How to end port 8080 so you can rerun it again:

``` netstat -ano | findstr :8080 ```

### OR

``` fuser 8080/tcp ```

### OR

``` lsof -i:8080 ```


### THEN:

``` kill <PID> ```

### OR (an all in one)

``` kill $(lsof -t -i:8080) ```
