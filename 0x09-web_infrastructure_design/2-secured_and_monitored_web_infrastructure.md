<h1>Distributed Web Infrastructures Design</h1>
<img src="2-secured_and_monitored_web_infrastructure.png" />
<a herf="https://miro.com/app/board/uXjVPj_HF6g=/"> Visit Online Board</a>
<h1>
    Description
</h1>
<p>
    This is a 3-server web infrastructure design that is secured, monitored, and serves encrypted traffic over https.
</p>
<h1>
    Specifics About This Infrastructure Design
</h1>
<ul>
<li>
    The purpose of the firewalls.
    The firewalls are for protecting the network (web servers, anyway) from unwanted and unauthorized users by acting as an intermediary between the internal network and the external network and blocking the incoming traffic matching the aforementioned criteria.
</li>
<li>
    The purpose of the SSL certificate.
    The SSL certificate is for encrypting the traffic between the web servers and the external network to prevent man-in-the-middle attacks (MITM) and network sniffers from sniffing the traffic which could expose valuable information. The SSL certs ensure privacy, integrity, and identification.
</li>
<li>
    The purpose of the monitoring clients.
    The monitoring clients are for monitoring the servers and the external network. They analyse the performance and operations of the servers, measure the overall health, and alert the administrators if the servers are not performing as expected. The monitoring tool observes the servers and provides key metrics about the servers' operations to the administrators. It automatically tests the accessibility of the servers, measures response time, and alerts for errors such as corrupt/missing files, security vulnerabilities/violations, and many other issues.
</li>
</ul>
<h1>
Issues With This Infrastructure
</h1>
<ul>
<li>
    Terminating SSL at the load balancer level would leave the traffic between the load balancer and the web servers unencrypted.
</li>
<li>
    Having one MySQL server is an issue because it is not scalable and can act as a single point of failure for the web infrastructure.
</li>
<li>
    Having servers with all the same components would make the components contend for resources on the server like CPU, Memory, I/O, etc., which can lead to poor performance and also make it difficult to locate the source of the problem. A setup such as this is not easily scalable.
</li>