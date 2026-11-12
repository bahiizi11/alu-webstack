# alu-webstack

My web infrastructure projects, built on three Ubuntu servers (two web servers and a load balancer).

## https_ssl

Making `www.arsenetech.tech` secure end to end.

- **0-world_wide_web**: a Bash script that uses `dig` and `awk` to show where each subdomain points.
- **1-haproxy_ssl_termination**: HAProxy config that handles HTTPS on port 443 with a Let's Encrypt certificate, then passes plain traffic to the web servers.
- **2-redirect_http_to_https**: HAProxy config that sends all HTTP visitors to HTTPS with a 301 redirect.
