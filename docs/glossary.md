# Glossary

A quick reference for the domain and DNS terms used across this repository. Definitions
follow the learning path in [LEARN.md](../LEARN.md); the book's own full glossary chapter
is [Glossary](../documents/tutorial/advanced/glossary.md).

## Names and zones

- **Domain** — A name in the DNS hierarchy. Here it usually means a registered name that
  has been delegated to external authoritative nameservers.
- **Subdomain** — A name below another domain, such as `www.example.dpdns.org`
  (see [Root Domains and Subdomains](../documents/tutorial/dns/2.2-subdomains.md)).
- **Zone** — The portion of the DNS namespace published as one administrative unit by
  authoritative nameservers.
- **Namespace** — A managed naming area or suffix under which names may be registered.
- **Registrant** — The person or organization that registers and is responsible for a domain.
- **Registrar / registration service** — The system through which a registrant creates and
  manages a domain registration.
- **Delegation** — The parent-zone records that identify the authoritative nameservers for
  a child zone (see
  [Delegation and External Nameservers](../documents/tutorial/dns/2.0-delegation.md)).
- **Authoritative nameserver** — A DNS server that publishes official data for a zone.
- **Recursive resolver** — A DNS server that follows referrals and caches answers for clients.
- **Glue record** — An address record supplied by a parent zone when it is needed to reach
  an in-zone nameserver.
- **WHOIS** — A legacy registration data lookup protocol, and a general term still used
  for domain registration information.
- **RDAP** — A structured protocol for accessing registration data.

## DNS records

Covered in depth in [DNS Record Types](../documents/tutorial/dns/2.1-record-types.md).

- **A record** — Maps a name to an IPv4 address.
- **AAAA record** — Maps a name to an IPv6 address.
- **CNAME** — Aliases one hostname to another canonical hostname.
- **NS record** — Identifies an authoritative nameserver.
- **MX record** — Identifies the mail exchangers for a domain.
- **TXT record** — Text data, commonly used for verification and email policy.
- **SRV record** — Identifies the hostname and port for a named service.
- **CAA** — A record that restricts which certificate authorities may issue certificates
  for a name.
- **SOA record** — The record containing core authority and timing information for a zone.
- **TTL (Time to Live)** — The maximum caching lifetime advertised with a DNS record
  (see [TTL, Caching, and Propagation](../documents/tutorial/dns/2.3-ttl-and-propagation.md)).

## Email records

See [Email DNS: MX, SPF, DKIM, and DMARC](../documents/tutorial/email/4.1-email-dns.md).

- **SPF** — An email authorization policy describing which systems may send using a domain
  in the SMTP envelope.
- **DKIM** — An email authentication method that uses a domain-published public key to
  validate message signatures.
- **DMARC** — An email policy and reporting mechanism based on SPF or DKIM authentication
  alignment with the visible From domain.

## Web and security

- **HTTP** — The application protocol used to request and deliver web resources.
- **HTTPS** — HTTP carried over TLS, providing transport encryption and server
  authentication (see [Enable and Verify HTTPS](../documents/tutorial/website/3.6-https.md)).
- **TLS** — The protocol that protects HTTPS and other network connections with encryption
  and authentication.
- **ACME** — A protocol for automating certificate issuance, validation, and renewal.
- **Proxy** — A system that receives traffic and forwards it to another service; it changes
  the network path and can affect logging, certificates, security, and policy.
- **Virtual host** — A web server configuration that selects a site based on the requested
  hostname.

For the documentation map, see the [documentation index](README.md).
