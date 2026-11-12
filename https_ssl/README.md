# https_ssl

Making `www.arsenetech.tech` secure end to end, on two web servers and a load balancer.

- **0-world_wide_web**: Bash script using `dig` and `awk` to show where each subdomain points.
- **1-haproxy_ssl_termination**: HAProxy config that terminates HTTPS on port 443 with a Let's Encrypt certificate.
- **2-redirect_http_to_https**: HAProxy config that redirects all HTTP traffic to HTTPS with a 301.
