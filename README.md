# Email Writer AI — Backend

Stateless, privacy-first backend for **Email Writer AI**, a browser extension + web app that generates AI-powered email replies. [Chrome Extension](https://chromewebstore.google.com/detail/email-writer/nefgnkboedlacmpgbkgjoknjeigpppln) · [Frontend repo](https://github.com/icas00/AI-Email-Writer-frontend)

## Tech Stack
- **Java, Spring Boot** — REST API
- **Gemini API** — AI reply generation
- **Railway** — deployment

## Design
- **Privacy-first**: the backend proxies AI requests without persisting any user data — zero email storage on the server.
- Exposes a simple REST endpoint that the [Chrome extension frontend](https://github.com/icas00/AI-Email-Writer-frontend) calls with extracted email context to generate a reply.
- Optimized request payloads to keep round-trip latency low.

## Getting Started
```bash
./mvnw spring-boot:run
```
Set your Gemini API key via environment variables before running.

## Related
- Frontend / Chrome extension: [AI-Email-Writer-frontend](https://github.com/icas00/AI-Email-Writer-frontend)
- Privacy policy: [email-writer-privacy](https://github.com/icas00/email-writer-privacy)

## License
MIT — see [LICENSE](LICENSE).
