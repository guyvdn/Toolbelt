# Seq

[Seq](https://datalust.co/seq) is built for modern structured logging with message templates. Rather than waste time and effort trying to extract data from plain-text logs with fragile log parsing, the properties associated with each log event are captured and sent to Seq in a clean JSON format. Message templates are supported natively by ASP.NET Core, Serilog, NLog, and many other libraries, so your application can use the best available diagnostic logging for your platform.

## Install into Docker desktop

```shell
docker run -d --restart unless-stopped --name seq -e ACCEPT_EULA=Y -v C:\Temp\Logs:/data -p 8081:80 datalust/seq:latest
``` 