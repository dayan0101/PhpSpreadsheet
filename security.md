# Security

APIs are increasingly vulnerable to security attacks. But the truth is that most threats can be prevented and avoided. That is why on our platform we use security protocols that allow us to avoid most threats.

## HTTPS secure connections

At ePayco all services are forced to HTTPS using TLS, including our public website and our dashboard. The details of our implementations are regularly audited, including the certificates authorizing their use and the encryption they support. HSTS is used to ensure that browsers interact with ePayco over HTTPS only.

## Encryption of sensitive data and communications

All credit card data is encrypted and a token card is generated for each of them, which is used for future transactions. The keys to decrypt are stored on separate machines. No one at ePayco can obtain your sensitive data. In ePayco, the infrastructure for storing, decrypting and sending credit card data runs in separate environments and they are not shared with anyone or in primary services \(API, website and others\).

## Parameters validation

In the API of our platform, in addition to the communication protocols and data encryption, we validate all incoming data, verifying its format, its validity and guaranteeing that it cannot cause damage to the system. We use a JSON serializer to correctly encode the data sent by the client and avoid the execution of code included within the information entered by the client.

