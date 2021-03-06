# Troubleshooting

We collect the most common troubleshooting of using Knowage for your reference:

> Instance troubleshooting is closely related to the Instance provider that is Cloud Platform, refer to [Cloud Platform Documentation](https://support.websoft9.com/docs/faq/tech-instance.html)

#### How can I use the logs?

You can find the keywords **Failed** or **error** by the command: `docker logs knowage-server`

#### Knowage service can't start?

Insufficient disk space, insufficient memory, and configuration file errors can make service could not be started  

It is recommended to first check through the command.

```shell
# restart Knowage service
docker restart knowage-server
docker logs knowage-server

# view disk space
df -lh

# view memory rate
free -lh
```