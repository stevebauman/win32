---
Description: A trust must exist between the recipient of a signed message and the signer of the message.
ms.assetid: 770e4674-8896-4062-a93a-a17bd30a9129
title: Certificate Trust Verification
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Certificate Trust Verification

A trust must exist between the recipient of a signed message and the signer of the message. One method of establishing this trust is through a [*certificate*](https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb), an electronic document verifying that entities or persons are who they claim to be. A certificate is issued to an entity by a third party that is trusted by both of the other parties. So, each recipient of a signed message decides if the issuer of the signer's certificate is trustworthy. [*CryptoAPI*](https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb) has implemented a methodology to allow application developers to create applications that automatically verify certificates against a predefined list of trusted certificates or [*roots*](https://msdn.microsoft.com/ce589e18-02ac-42c2-b76b-776deb686bbd). This list of trusted entities (called subjects) is called a [*certificate trust list*](https://msdn.microsoft.com/db46def4-bfdc-4801-a57d-d568e94a2dbb) (CTL).

The following example of using a CTL involves an intranet (intra-company network) administrator who wants to control just which outside sources are trusted. In this case, the administrator can create a list of trusted certificates or roots, sign it, and make the list available to all clients on the network in the form of a CTL. An application designed to use this CryptoAPI functionality would then only accept signed messages or downloaded software that was signed by entities on the list.

For a list of these functions, see [Certificate Verification Functions](cryptography-functions.md).

 

 


