# Wallarm Solutions Engineer Summary - Barry Kemble

## 📌 Task Summary 

I reviewed the Challenge and given the subscription I had assigned to me and other available resources ruled out a number of scenarios and settled on Nginx with All-in-one Installer.

Built this out using my ProxMox Lab with DNS, NAT and SSL certificates to give a real world feel to the deployment as if it were a true internet facing setup.

See included high level diagram.

Wallarm was configured as a Node and connected to the Wallarm Dashboard however I did miss the Nginx directives on Step 5 whilst troubleshooting Nginx and Certbot issues as my Nginx lab had been used to front something else on my network.

Running gotestwaf was not being blocked and once I worked out that my Nginx was not invoking Wallarm this was remedied and I moved on with the testing with gotestwaf.

Please see included report.

The filtering node is correctly blocking traffic and this can be seen in the Dashboard.

I made significant use of the official documentation to get a feel for how the product works, configuration for Wallarm and Nginx and overall guidelines.

Also interesting to look at the Nginx logs and see the number of IP addresses randomly trawling my DNS record.

See screenshot of interesting ip’s.

## Lessons Learnt
Perhaps a Greenfield Nginx deployment would be better next time to reduce the troubleshooting 😎.







