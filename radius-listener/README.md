# MyGaru Radius Listener
MyGuru Account Catcher listens for RADIUS notifications within the telecom couture and passes them ~~to RabbitMQ (old version)~~ directly to the IDR client for further processing (simplified version for testing).
MyGuru Account Catcher processes only ``` CodeAccountingRequest ``` packet code.
Data grabbing and delivery is implemented using so-called catchers and notifiers.

# Before start
Radius Listener doesn't require 433/80 ports. By default app listens port :8080 
```shell
httpServerListenAddr = :8080
```

Radius UDP settings must be specified
```shell
radiusListenUDPAddr = :11813
radiusUsernameSalt = f1nd1ngn3m0
```

During the test setup, the Radius Listener communicates with the IDR client directly without the Map Store UID. 
Plase, specify the IDR host using the parameter:

```shell
idrTestHost = example.com
```

# How to launch?
```shell
./rcatcher --config=config.ini
```
