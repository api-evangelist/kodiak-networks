# Kodiak Networks

Kodiak Networks built a carrier-grade Push-to-Talk over Cellular (PoC) platform that wireless operators deployed as their own branded push-to-talk service, competing with legacy land mobile radio for dispatch, field-service and public-safety workforces.

**Status: acquired.** Motorola Solutions acquired Kodiak Networks in 2017. The technology ships today as Motorola Solutions' [Kodiak mission-critical PTT for carriers](https://www.motorolasolutions.com/en_us/products/command-center-software/broadband-ptt-and-lmr-interoperability/mcptt-deployment.html), aligned to the 3GPP SA WG6 MCPTT specifications (TS 23.379, TS 24.382, TS 24.482, TS 22.582) and interoperable with LMR via Critical Connect.

## API surface

Kodiak Networks publishes **no public API surface**. The legacy domain http://www.kodiaknetworks.com/ serves a static "Site under maintenance" placeholder over plain HTTP (no TLS listener), and every `/.well-known/` and spec path probes 404.

Broadband push-to-talk APIs for third-party integration do exist, but access is gated:

- [Application Developer Program](https://www.motorolasolutions.com/en_us/developers/application-partner-developer-program.html) — the program granting access to Broadband Push-to-X APIs
- [API partner onboarding](https://partnerapply.motorolasolutions.com/s/api-partner-onboarding-new-application?language=en_US) — the sign-up path
- [code.motorolasolutions.com](https://code.motorolasolutions.com/users/sign_in) — partner developer portal (sign-in required)

## Artifacts

- `llms/kodiak-networks-llms.txt` — generated llms.txt profile
- `security/kodiak-networks-domain-security.yml` — probed TLS/DNS posture
- `well-known/kodiak-networks-well-known.yml` — negative `/.well-known/` probe record

Backed by: redpoint-ventures
