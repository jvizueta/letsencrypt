# letsencrypt
```
root@omv:~# acme.sh --server letsencrypt \
  --issue \
  -d mydomain.com \
  -d '*.mydomain.com' \
  -d '*.omv.mydomain.com' \
  --dns dns_manual \
  --dnssleep 120 \
  --yes-I-know-dns-manual-mode-enough-go-ahead-please
[Mon May  5 10:44:58 AM WEST 2025] Using CA: https://acme-v02.api.letsencrypt.org/directory
[Mon May  5 10:44:58 AM WEST 2025] Multi domain='DNS:mydomain.com,DNS:*.mydomain.com,DNS:*.omv.mydomain.com'
[Mon May  5 10:45:03 AM WEST 2025] Getting webroot for domain='mydomain.com'
[Mon May  5 10:45:03 AM WEST 2025] Getting webroot for domain='*.mydomain.com'
[Mon May  5 10:45:03 AM WEST 2025] Getting webroot for domain='*.omv.mydomain.com'
[Mon May  5 10:45:04 AM WEST 2025] Cannot find DNS API hook for: dns_manual
[Mon May  5 10:45:04 AM WEST 2025] You need to add the TXT record manually.
[Mon May  5 10:45:04 AM WEST 2025] Add the following TXT record:
[Mon May  5 10:45:04 AM WEST 2025] Domain: '_acme-challenge.mydomain.com'
[Mon May  5 10:45:04 AM WEST 2025] TXT value: 'XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'
[Mon May  5 10:45:04 AM WEST 2025] Please make sure to prepend '_acme-challenge.' to your domain
[Mon May  5 10:45:04 AM WEST 2025] so that the resulting subdomain is: _acme-challenge.mydomain.com
[Mon May  5 10:45:04 AM WEST 2025] Cannot find DNS API hook for: dns_manual
[Mon May  5 10:45:04 AM WEST 2025] You need to add the TXT record manually.
[Mon May  5 10:45:04 AM WEST 2025] Add the following TXT record:
[Mon May  5 10:45:04 AM WEST 2025] Domain: '_acme-challenge.mydomain.com'
[Mon May  5 10:45:04 AM WEST 2025] TXT value: 'YYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYYY'
[Mon May  5 10:45:04 AM WEST 2025] Please make sure to prepend '_acme-challenge.' to your domain
[Mon May  5 10:45:04 AM WEST 2025] so that the resulting subdomain is: _acme-challenge.mydomain.com
[Mon May  5 10:45:04 AM WEST 2025] Cannot find DNS API hook for: dns_manual
[Mon May  5 10:45:04 AM WEST 2025] You need to add the TXT record manually.
[Mon May  5 10:45:04 AM WEST 2025] Add the following TXT record:
[Mon May  5 10:45:04 AM WEST 2025] Domain: '_acme-challenge.omv.mydomain.com'
[Mon May  5 10:45:04 AM WEST 2025] TXT value: 'ZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZZ'
[Mon May  5 10:45:04 AM WEST 2025] Please make sure to prepend '_acme-challenge.' to your domain
[Mon May  5 10:45:04 AM WEST 2025] so that the resulting subdomain is: _acme-challenge.omv.mydomain.com
[Mon May  5 10:45:04 AM WEST 2025] Please add the TXT records to the domains, and re-run with --renew.
[Mon May  5 10:45:04 AM WEST 2025] Please add '--debug' or '--log' to see more information.
[Mon May  5 10:45:04 AM WEST 2025] See: https://github.com/acmesh-official/acme.sh/wiki/How-to-debug-acme.sh
root@omv:~#
```
