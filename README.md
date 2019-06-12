# Agents
This is the main repository for all interfaces for battle.ai

In general each game defines an interface using [grpc.io](https://grpc.io). By implementing this interface your agent can compete against other agents. 

Please see the folders for details on each game

 * [Connect Four](connect-four)

### Running agents locally

If your localhost does not have a publicly available IP address you can use
`ssh -R 0:localhost:5001 serveo.net` to get a publicly accessible `host:port` that maps to your `localhost:5001`.
 
For instance

```
$ ssh -R 0:localhost:5001 serveo.net
Allocated port 38234 for remote forward to localhost:5001
Forwarding TCP connections from serveo.net:38234
```

Means requests to  `serveo.net:38234` is routed to your `localhost:5001` where your agent is listening.
