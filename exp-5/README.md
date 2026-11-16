# Experiment 5: Network Traffic Privacy and Session Security

## Aim

To inspect protocol metadata in a packet capture and explain how encryption and secure session management reduce the risk of traffic interception.

## Scope and Safety

Use only a packet capture supplied by your instructor or created on an isolated lab network that you control. Do not capture other people's traffic, collect real credentials, or attempt to take over a session. This exercise is observational and does not perform session hijacking.

## Tools

- Wireshark
- An instructor-provided or self-created lab capture (`.pcap` or `.pcapng`)

## Procedure

1. Open the authorized lab capture in Wireshark.
2. Record the capture's interface or source, time range, and the protocols listed in **Statistics > Protocol Hierarchy**.
3. Use display filters such as `dns`, `tcp`, and `tls` to compare protocol metadata. Note that encrypted application content should not be readable from a capture alone.
4. Select a TLS packet and review its handshake and certificate metadata. Do not attempt to decrypt traffic or access session tokens.
5. In your report, describe at a high level how an exposed or stolen session token could be misused, without attempting to obtain or replay one.
6. Recommend protections: HTTPS throughout the session, `Secure`, `HttpOnly`, and appropriate `SameSite` cookie attributes, session rotation after authentication or privilege changes, short inactivity timeouts, and server-side logout invalidation.

## Observation Table

| Item | Observation |
|---|---|
| Capture source and authorization | |
| Protocols observed | |
| Evidence of encrypted application traffic | |
| Sensitive data intentionally excluded | |
| Recommended session protections | |

## Result

The capture was reviewed for protocol metadata, and the report identified how encryption and secure cookie/session handling help protect users. No credentials or live sessions were collected or accessed.

## Conclusion

Packet analysis can reveal useful network metadata even when application content is encrypted. Session security depends on protecting tokens in transit and enforcing safe token handling on the server.
