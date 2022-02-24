# Quick reference

-	**Maintained by**:  
	[PilotFish Technology, LLC](https://www.pilotfishtechnology.com)

-	**Where to get help**:  
	[PilotFish Technology CMS](https://cms.pilotfishtechnology.com)

# What is eiPlatform?
The eiPlatform enterprise integration solution is a complete Java framework that leverages application server technology, web services and industry XML standards to enable the deployment of internal and external system interfaces better, faster and less expensively than ever before possible. When combined with the graphical IDE component, the eiConsole, the developer has the most comprehensive solution for enterprise integration.

[www.pilotfishtechnology.com/enterprise-integration-platform/](https://www.pilotfishtechnology.com/enterprise-integration-platform/)

![logo](https://www.pilotfishtechnology.com/wp-content/uploads/2015/03/pilotfish-logo.png)

## Quick Setup

1. Install Docker

- [Docker Install documentation](https://docs.docker.com/install/)

2. Clone the main branch of the repository

```bash
cd /opt
git clone https://github.com/pilotfishtechnology/eiplatform_quick_start
cd eiplatform_quick_start
```

3. Log in to the [Pilotfish Customer Portal](https://customerportal.pilotfishtechnology.com/portal/login.html) and download your latest license file.

4. Copy in your license file (`pflicense.key`) with your latest routes (`eip-root`).

5. Bring up your stack by running

```bash
sh start.sh
```

When your docker container is running, connect to it on port `8080` to access the eiplatform instance.
Sometimes this can take a little bit because of the entropy of keys.

[http://127.0.0.1:8080/eip/](http://127.0.0.1:8080/eip/)
