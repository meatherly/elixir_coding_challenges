# TCP Chat

In this challenge you'll build a tcp chat app. Your clients will be able to connect with a client like telnet.

The server should be able to do the follow:

1. Upon connecting prompt the client for their nickname.
    * This nickname is case-sensitive and must be unique on the server.
    * If the nickname is already taken the server should tell the user to choose a new nickname.
2. Upon entering a valid nickname, the server should:
    * Send the last 10 lines of chat in the chat-room,
    * Broadcast that the user has connected to the other clients
    * Send a list of users that are currently connected to the just-connected client.
3. Upon disconnecting, the server should:
    * Broadcast that the user has disconnected.
4. If the user is "@mentioned", meaning the message contains @theirnickname, a BEL (`'\a'`) character should be sent to the client that is connected with that nickname.

## Working Example
You don't need to include `<` and `>` They are there to show the direction of the message in the example.
```
< Welcome to my chat server! What is your nickname?
> Jake
< You are connected with 3 other users: [bill, bob, jim]
< [12:04:05] <bill> yo
< [12:04:06] <bill> whats up?
< [12:04:07] <bob> nothing much!
< [12:04:09] *Jake has joined the chat*
> Hey whats going on guys?
< [12:06:09] <bill> Nothing much!!
```

## Helpful links
* [TCP Server tutorial](https://elixir-lang.org/getting-started/mix-otp/task-and-gen-tcp.html)
* [gen_tcp Erlang docs](http://erlang.org/doc/man/gen_tcp.html)
* [Quick guide on telnet](https://www.computerhope.com/unix/utelnet.htm)

## Extra Challenges
* Use ANSI escape codes to colorize the text and bold @mentions


Credit goes to [Discord](https://github.com/discordapp) for giving me this challenge.