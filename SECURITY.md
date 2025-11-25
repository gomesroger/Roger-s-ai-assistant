# Security Policy

## Implemented Protections

- **Server-side rate limiting**: 5 requests per IP per 10 minutes
- **Input sanitization**: All user inputs are validated and cleaned
- **Honeypot trap**: Hidden field detects bot submissions
- **Request signing**: Timestamped tokens prevent replay attacks
- **Email validation**: Regex + format checks on both client and server
- **Spam detection**: Keyword filtering for common spam patterns

## Known Limitations

This is a client-side application with an exposed backend endpoint. 
While multiple layers of protection exist, determined attackers could:
- Bypass client-side validation by crafting direct API requests
- Spam the endpoint from distributed IPs

## Responsible Disclosure

If you discover a security vulnerability, please email: security@yourdomain.com
