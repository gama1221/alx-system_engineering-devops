<img src="0-simple_web_stack.md.png" />
<a href="https://miro.com/app/board/uXjVPj4aDlo=/">Visit online Bord</a>
<h1>
    Description
</h1>
This is a simple web infrastructure that hosts a website that is reachable via www.foobar.com/8.8.8.8 ip address.
<h1>
    Specifics About This Infrastructure
</h1>
<ul>
    <li><strong> Server? </strong>.</li>
    <p> A server is a <i>powerful</i> computer hardware or software that provides different services to other computers, which are usually referred to as clients or users.
    </p>
    <li><strong>DNS </strong></li>
    <p>
       It is a naming system for computers, services, and other resources in the Internet or other Internet Protocol networks For example, the domain name                      www.ethiopianairlines.com is easier to recognize and remember than [23.12.103.180]. The IP address and domain name alias is mapped in the Domain Name System (DNS)
        The type of DNS record www is in www.foobar.com.
        www.foobar.com uses an A record. This can be checked by running dig www.foobar.com.
        Note: the results might be different but for the infrastructure in this design, an A record is used.
        Address Mapping record (A Record)—also known as a DNS host record, stores a hostname and its corresponding IPv4 address.
    </p>
<li>
    <strong>The role of the web server</strong>
</li>
    <p>
    The web server is a software/hardware that accepts requests via HTTP or secure HTTP (HTTPS) and responds with the content of the requested resource or an error messsage.
    </p>

<li>
    <strong> The role of the application server </strong>
    <p>
    To install, operate and host applications and associated services for end users, IT services and organizations and facilitates the hosting and delivery of high-end consumer or business applications
    </p>
    <li><strong>The role of the database.</strong>
        <p>
To maintain a collection of organized information that can easily be accessed, managed and updated

What the server uses to communicate with the client (computer of the user requesting the website).
Communication between the client and the server occurs over the internet network through the TCP/IP protocol suite.
        </p>
        </ul>
<h1> Issues With This Infrastructure Design </h1>
<p>
<ul><li>
    There are multiple SPOF (Single Point Of Failure) in this infrastructure.
For example, if the MySQL database server is down, the entire site would be down.
    </li>
    <li>
Downtime when maintenance needed.
When we need to run some maintenance checks on any component, they have to be put down or the server has to be turned off. Since there's only one server, the website would be experiencing a downtime.
    </li>
    <li>
Cannot scale if there's too much incoming traffic.
It would be hard to scale this infrastructure becauses one server contains the required components. The server can quickly run out of resources or slow down when it starts receiving a lot of requests.
    </li>
    </ul>
