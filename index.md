# Sunsetting dotHIV Domain Hosting Services

When we launched the digital red ribbon in 2014 a lot of our work went into making it as easy as possible for domain owners to show [the ribbon](https://github.com/dothiv/ribbon) on their domain. We did this through providing DNS and webhosting services through [Google Cloud](https://cloud.google.com/), [CloudFlare](https://www.cloudflare.com/) and [GitHub pages](https://pages.github.com/)—free of charge.

> In 2020 we are sunsetting this offering and we will end its support on 31st of December 2020. 

Please review the migration instructions below carefully and migrate your .HIV as soon as possible.

In short:
- use your own DNS service (e.g. [deSEC](https://desec.io/) or [CloudFlare](https://www.cloudflare.com/))
- use your own webhosting service (e.g. [GitHub pages](https://pages.github.com/))

If you need further assistance, please do not hesitiate to reach out to our CTO Markus [via email](mailto:m@tld.hiv) or [via Twitter](https://twitter.com/coderbyheart).

## Migrating to your Nameserver and webhosting services

### 1. Point the nameserver records of your HIV domain to your own service

In the past we asked you to use CloudFlare's nameserves, e.g. `bill.ns.cloudflare.com`. In case you want to keep using [CloudFlare](https://www.cloudflare.com/) sign up for a free account there and add your .HIV domain to your account.

Otherwise, go to your domain registrars control panel of your domain and enter the hostnames provided by your nameserver service. Typically your registrar can provide them for you.

### 2.  Point the CNAME and A records to your own webhosting service

In the past we asked you to use GitHub's IPs in your A records and `dothiv.github.io` for the `www` CNAME record:
```
example.hiv. A 185.199.108.153  
example.hiv. A 185.199.109.153  
example.hiv. A 185.199.110.153  
example.hiv. A 185.199.111.153  
www.example.hiv. CNAME dothiv.github.io
```

In case you want to keep using the GitHub pages services, please add these records to your domain using your DNS provides control panel (remember to replace `example.hiv` with your .hiv domain).

If you want to make modifications to this website, please contact us so we can transfer the ownership of the repository to your GitHub organization. For example, [this](https://github.com/dothiv/register.hiv) is the GitHub repository for [register.hiv](https://register.hiv/).

Otherwise enter the records provided to you by your webhosting service.

## Timeline

### January 2020

Announcement of Sunsetting.

### December 31st 2020

- Removal of Zones hosted on Google Cloud DNS (`ns-cloud1.googledomains.com`, `ns-cloud2.googledomains.com`, `ns-cloud3.googledomains.com`, `ns-cloud4.googledomains.com`)

<!--stackedit_data:
eyJoaXN0b3J5IjpbMjAyMDA1NTkwNiwyMzg5MDE2NTAsMTMwNT
A0NDkwNV19
-->