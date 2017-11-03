additionally, listing the config of krb5.conf 
```
[logging]
 default = FILE:/var/log/krb5libs.log
 kdc = FILE:/var/log/krb5kdc.log
 admin_server = FILE:/var/log/kadmind.log

[libdefaults]
 default_realm = NithK45.FNG
 dns_lookup_realm = false
 dns_lookup_kdc = false
 ticket_lifetime = 24h
 renew_lifetime = 7d
 forwardable = true
default_tgs_enctypes = aes256-cts-hmac-sha1-96 aes128-cts-hmac-sha1-96 arcfour-hmac-md5
 default_tkt_enctypes = aes256-cts-hmac-sha1-96 aes128-cts-hmac-sha1-96 arcfour-hmac-md5
 permitted_enctypes = aes256-cts-hmac-sha1-96 aes128-cts-hmac-sha1-96 arcfour-hmac-md5


[realms]
 NithK45.FNG = {
  kdc = ip-172-31-43-3.us-west-2.compute.internal
  admin_server = ip-172-31-43-3.us-west-2.compute.internal
 }

[domain_realm]
 .example.com = NithK45.FNG
 example.com = NithK45.FNG
```