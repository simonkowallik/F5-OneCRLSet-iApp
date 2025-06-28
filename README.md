# This iApp

This iApp allows integration of CRLSet and OneCRL into F5 BIG-IP, specifically F5 SSLO.

## CRLSet and OneCRL: What, why and how

CRLSet and OneCRL are certificate revocation systems developed by Google and Mozilla to address the performance and reliability problems of traditional revocation checking methods such as CRLs and OCSP.

The purpose of both systems is to allow browsers to identify and block untrustworthy SSL/TLS certificates without having to perform slow, live online checks for every connection.

Google's CRLSet is designed for the fast, emergency revocation of specific website certificates. It allows a quick response to immediate threats. Mozilla's OneCRL, on the other hand, focuses on the structural risk of compromised intermediate certificates. Such certificates can be misused to issue fraudulent but trusted certificates for countless domains.

Both systems provide a practical answer to the otherwise "broken" state of certificate revocation, where high latency, limited reliability and privacy concerns remain common problems.

By distributing revocation lists directly to the browser, CRLSet and OneCRL enable fast, local checks. This improves security and performance, especially when responding to serious incidents such as a compromised intermediate CA certificate or a fraudulent end-entity certificate.

## F5 SSL Orchestrator: Unifying certificate revocation checking

By integrating Google's CRLSet and Mozilla's OneCRL, F5 SSL Orchestrator brings both approaches together at one central, **network-wide** enforcement point.

This is a game-changer. It closes the gap between browser and network security and combines two complementary methods. Together, they cover different, critical types of certificate risk rather than addressing only one part of the problem.

