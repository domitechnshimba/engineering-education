# What is WebSocket?

Hello guys, welcome back again for another interesting and educational article.

Today, we are going to taking a dive into a very cool **JavaScript API** that improves the way the Web Browser communicates with the Server.

This **JavaScript API** is called **Websocket**. (just before I start talking about Websocket, incase you don't know what a server is):

_A **Server** is simply a software or hardware device that accepts and responds to requests made over a Network._

These requests might be for HTML files or whatsoever. I know you might be having thoughts like:

_"Does it really matter?"_

_"**HTTP/HTTPS** communications are good enough"._

Well, communications using **HTTP/HTTPS Protocol** can be good at times, depending on the project at hand.

Some day, you might wake up wanting to create a website that sends out and receives a lot of data, and that day you might consider or have no other option than to use **Websocket**. 

But, What is this **Websocket** that tends to improve the communication between the Client(browser) and the Server?

_**WebSocket** is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.(- Wikipedia)._

Let me explain...

A communication using Websocket is more like the browser giving the Server a call and both of them are like:-

_**Browser:**  "Hey Server, update Sam's name to Incognito"._

_***Server:** "Done"._

_**Server:** "Incognito has a message from Jubilee"._

_**Browser:** "Okay"._

While a communication using the **HTTP/HTTPS protocol** from a Browser to the Server might be like the Browser sending the Server an SMS. Here is an illustration.

_**Browser:** "Hey Server, update Sam's name to Incognito"._

_**Server:** "Done"._

_**Browser:** "Any new updates?"_

_**Server:** "Yes, Incognito has a message from Jubilee"._

_**Browser:** "Okay"._

In the communication using **HTTP/HTTPS protocol**, one thing is quite obvious, which is that the Browser has to send a request before the server responds. In this case, the Server is not a big mouth and does not blab what it's not asked.

While in the communication using _**Websocket**_, the _**Server**_ and the _**Browser**_ can communicate freely (blabbing as you might guess). The Server does not have to wait to be asked. Once it has something to say to the Browser, it says it and the Browser listens too.

This does not make **HTTP/HTTPS Protocol** bad, it still has its own benefits. If your Server is running a simple service like a voting system, you can use **HTTP/HTTPS Protocol** and it would work well.

**Websocket** is usually used when the Server is running for example:

An online game that requires users to send and receive a lot of requests and let those requests interact with the Server at anytime all throughout the game without pushing any other button.

It's either the Server is asked once, or the Server is never asked (provided the Server is connected to the client) but gives needed responses.

_Cool right?_

Also, remember that the Server is not just communicating with one browser, it is communicating with many.

So, in a situation where the **HTTP/HTTPS Protocol** is used in place of a Websocket, the Browser might end up bombing the Server causing a DOS(Denial of Service) attack.

This might happen when the smart programmer wraps the request with an interval too fast like (1 millisecond) in order to get responses faster and try to replicate live requests and responses.

_One of the Social Media networks that use **Websocket** is **Telegram.**_

**Telegram** is a very fast instant messaging application and telegram group chats can have up to 10,000 people in it and if only 500 people are chatting in it at a time, it will still be faster than a Facebook group chat with 30 people chatting on it.

This is because Facebook uses **HTTP/HTTPS Protocol** and wraps it in a time interval.

_One of the benefits of **Websocket** that I love so much is that it saves Data._

A site using **HTTP/HTTPS Protocol** will keep sending requests even when there are no responses and these requests do burn data.

Using **WebSocket** solves this problem because it sends and receives data only when needed. And that's it's for this article. Hope it's clear.