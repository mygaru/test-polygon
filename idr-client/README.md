# MyGaru IDR Client
IDR Client/Decrypter is a single application responsible for OTP encoding/decoding.
The internal/private version is deployed on the Telecom private network contour.

# Before start
Please specify the path to the HTTPS certificates in the configuration file
```shell
httpServerTLSCertFile = /somedomain.com.crt
httpServerTLSKeyFile = /somedomain.com.key
```

NOTE: IDR client listens 80 and 433 ports.

# How to launch?
```shell
./idrclient --config=config.ini
```
