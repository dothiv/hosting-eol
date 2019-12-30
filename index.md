# Sunsetting dotHIV Domain Hosting Services

When we launched the digital red ribbon in 2014 a lot of our work went into making it as easy as possible for domain owners to show the [ribbon](https://github.com/dothiv/ribbon) on their domain. We did this through providing DNS and webhosting services through [Google Cloud](https://cloud.google.com/), [CloudFlare](https://www.cloudflare.com/) and [GitHub pages](https://pages.github.com/)—free of charge.

> In 2020 we are sunsetting this offering and we will end it's support on 31st of December 2020. 

Please review the migration instructions below carefully and migrate your .HIV as soon as possible.

If you need further assistance, please do not hesitiate to reach out to our CTO Markus [via email](mailto:m@tld.hiv) or [via Twitter](https://twitter.com/coderbyheart).

## Migrating to your Nameserver and webhosting services

### 1. Point the nameserver records of your HIV domain to your own service

In the past we asked you to use CloudFlare's nameserves, e.g. `bill.ns.cloudflare.com`. In case you want to keep using [CloudFlare](https://www.cloudflare.com/) sign up for a free account there and add your .HIV domain to your account.

Otherwise, go to your domain registrars control panel of your domain and enter the hostnames provided by your nameserver service. Typically your registrar can provide them for you.

### 2.  Point the CNAME and A records to your own webhosting service

In the past we asked you to use GitHubs
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjA4MTgzNzA2MSwxMzA1MDQ0OTA1XX0=
-->