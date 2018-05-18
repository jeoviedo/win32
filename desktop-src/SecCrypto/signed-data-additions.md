---
Description: 'Lists the changes in capabilities of signed data.'
ms.assetid: '0518a336-d996-4a82-9336-a448284c72dd'
title: Signed Data Additions
---

# Signed Data Additions

The following changes have been made to signed data capabilities:

-   Nondata [*inner content*](security.i_gly#-security-inner-content-gly) is encapsulated in an OCTET STRING.
-   Provision is made for different message versions.
-   Signers can be identified either by Issuer and Serial Number, as in PKCS \#7 1.5, or by Subject key identifier.
-   Multiple signers are allowed.
-   Both RSA, DSA, and ECDSA signatures are allowed.
-   Elliptic Curve Cryptography (ECC) based algorithms and AES require Windows Vista or later.

 

 


