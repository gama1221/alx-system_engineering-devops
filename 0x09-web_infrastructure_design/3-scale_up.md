<img src="3-scale_up.jpg" alt="Please wait to display an image" />
<h1>
Description about this infractructure design
</h1>
<p>
    This web infrastructure is a scaled up version of the infrastructure described <a href="https://github.com/gama1221/alx-system_engineering-devops/blob/main/0x09-web_infrastructure_design/2-secured_and_monitored_web_infrastructure.md"> here </a>. In this version, all SPOFs have been removed and each of the major components (web server, application server, and database servers) have been moved to separate GNU/Linux servers. The SSL protection isn't terminated at the load-balancer and each server's network is protected with a firewall and they're also monitored
</p>
<h1>
    Specifics About This Infrastructure
</h1>
<ul>
    <li>
        The addition of a firewall between each server.
        This protects each server from unwanted and unauthorized users rather than protecting a single server.
    </li>
</ul>
<h1>
    Issues With This Infrastructure Design
</h1>
<ul>
<li>
    High maintenance costs.
    Moving each of the major components to its own server, means that more servers would have to be bought and the company's electricity bill would rise along with the introduction of new servers. Some of the company's funds would have to be used to buy the servers and pay for the electricity consumption needed to keep the servers (including the new and old ones) running.
</li>
</ul>
