# Did Verifier Static App

This is an example about how to configure a [workflow](https://docs.github.com/actions/) action to deploy a free [Static Web App in Azure](https://docs.microsoft.com/azure/static-web-apps)
to support the Decentralized Identifiers ([DID](https://w3c.github.io/did-core/)) verification for your [Verifiable Credentials](https://www.microsoft.com/security/business/identity-access-management/verifiable-credentials).

---

The DID [domain verification](https://docs.microsoft.com/azure/active-directory/verifiable-credentials/how-to-dnsbind#verified-domain) needs to find a [did-configuration.json](tree/main/html/.well-known) file in the .well-known folder in the root of your domain. So, this workflow uses
[project Oryx](https://github.com/Microsoft/Oryx) to deploy these files in a Static Web App that serves also a simple HTML index file for your domain.

