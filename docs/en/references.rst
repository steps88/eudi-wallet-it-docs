.. include:: ../common/common_definitions.rst

.. _defined-terms.rst:


Normative References
+++++++++++++

Below the normative references and respective acronyms included in these Technical Specifications: 

[CAD] 

Legislative Decree No. 82 of March 7, 2005, as amended, containing the 'Digital Administration Code'. 

 
[REF_ACCESSIBILITY]

Accessibility Guidelines for IT Tools as per Article 11 of Law 4/2004. 
Directive (EU) 2019/882 of the European Parliament and of the Council of 17 April 2019 on the accessibility requirements for products and services. 

 
[GL_DESIGN] 

Design Guidelines for  websites and digital services provided by public administrations, pursuant to Article 53, paragraph 1-ter of Legislative Decree No. 82 of March 7, 2005, as amended. 


Defined Terms and Acronyms
--------

The terms *User*, *Trust Service*, *Trust Model*, *Trusted List*, *Trust Framework*, *Attribute*, *Electronic Attestations of Attributes Provider* or *Trust Service Provider (TSP)*, *Person Identification Data (PID)*, *Revocation List*, *Qualified Electronic Attestations of Attributes Provider* or *Qualified Trust Service Provider (QTSP)*, *Electronic Attestation of Attributes (EAA)*, are defined in the `EIDAS-ARF`_.

Below are the description of acronyms and definitions which are useful for further insights into topics that complement the IT-Wallet System and the interacting components.

.. list-table::
   :header-rows: 1

   * - Name
     - Description
     - Notes
   * - Accreditation Process
     - Process performed by the National Accreditation Body to accreditate CABs. As a result of the Accreditation Process, a NAB issues an accreditation certificate to a CAB.
     - | 
   * - Authentication
     - Pursuant to Article 3, paragraph 1, point 5 of the eIDAS Regulation, an electronic process that enables the confirmation of the Electronic Identification of a natural or legal person, or the origin and integrity of data in electronic form (in the context of the Guidelines, for example, Attributes).
     - [According to LLGG]
   * - Authentic Source	
     - Public Entity or Private Entity responsible for the repository or system, considered a primary source for Attributes or for Personal Identification Data, and whose authenticity is recognized in accordance with Union or national law, including administrative practice.
     - [According to LLGG – definition merged with Authentic Source Holder]
   * - Attributes	
     - A set of characteristics, qualities, rights, or permissions of a natural or legal person, or of an object, or even a single piece of such information.	
     - [According to LLGG]
   * - Certification Process
     - Process performed by Conformity Assessment Bodies to certify the Wallet Solution. The Certification Process aims to periodically assess technical Wallet Solutions (e.g. performing vulnerability assessment and risk analysis). As a result of the Certification Process a certification is provided to the Wallet Solution.
     - 
   * - Conformity Assessment Body (CAB)
     - A conformity assessment body as defined in Article 2, point 13, of Regulation (EC) No 765/2008, which is accredited in accordance with that Regulation as competent to carry out conformity assessment of a qualified trust service provider and the qualified trust services it provides, or as competent to carry out certification of Wallet Solutions or electronic identification means.
     - Aligned with ARF v1.4.
   * - Critical Assets
     - They are assets within or in relation to a Wallet Unit (for example cryptographic keys) of such importance that their incapacitation or destruction would have a very serious, debilitating effect on the ability to rely on the Wallet Unit.
     - | Revised from Implementing Act.
       | 
       | *Differences:*  editorial.
   * - Credential Issuer 
     - An Organizational Entity providing Digital Credentials to Users. It may be PID Provider or (Q)EAA Providers.
     - | Revised from ARF v1.4.
       | 
       | *Differences:*  (i) merged the PID Providers and (Q)EEA Providers definitions using the general term Digital Credential, (ii) renamed “Member Stare or other legal entity” in “Organizational Entity” ARF alternative terms: PID Providers, (Q)EEA Providers, Attestation Provider.
       | *Alternative terms:* Verifiable Credential Issuer, Electronic Attestation Provider.
   * - Credential Status Assertion
     - Signed document serving as proof of a Digital Credential's current validity status.
     - 
   * - Cryptographic Hardware Key Tag
     - A unique identifier created by the operating system for the Cryptographic Hardware Keys, utilized to gain access to the private key stored in the hardware.
     - 
   * - Cryptographic Hardware Keys
     - During the app initialization, the Wallet Instance generates a pair of keys, one public and one private, which remain valid for the entire duration of the Wallet Instance's life. Functioning as a Master Key for the personal device, these Cryptographic Hardware Keys are confined to the OS domain and are not designed for signing arbitrary payloads. Their primary role is to provide a unique identification for each Wallet Instance.
     - 
   * - Device Integrity Service
     - A service provided by device manufacturers that verifies the integrity and authenticity of the app instance (Wallet Instance), as well as certifying the secure storage of private keys generated by the device within its dedicated hardware. It's important to note that the terminology used to describe this service varies among manufacturers.
     - 
   * - Digital Credential 
     - A signed set of Attributes encapsulated in a specific data format, such as mdoc format specified in [ISO 18013-5] or the SD-JWT VC format specified in [SD-JWT-VC]. This may be a Personal Identification Data (PID), (Qualified) Electronic Attestation of Attribute ((Q)EAA).
     - | Revised from ARF v1.4.
       | 
       | *Differences:*  The definition from ARF restricts the data format to mdoc and SD-JWT VC. A Digital Credential definition should be neutral on the format.
       | *Alternative terms:* Electronic Attestation, Attestation, Verifiable Credential, Digital Attestation.
   * - Digital Identity Provider
     - Entity responsible for identifying citizens for the issuance of a digital identity.
     - 
   * - Federation Authority
     - A public governance entity that issues guidelines and technical rules and administers - directly or through its intermediary - Trusted Lists, services, and accreditation processes, the status of participants, and their eligibility evaluation. It also performs oversight functions.
     - 
   * - IT-Wallet System
     - Set of Technical Solutions that implement the "Italian Digital Wallet System" pursuant to Article 64-quater of [CAD].
     - 
   * - IT-Wallet System Register
     - Register containing the list of Public Entities and Private Entities that are registered in the IT-Wallet System.
     - [According to LLGG]
   * - Holder
     - Natural or Legal person that receives Digital Credentials from the Credential Issuers, manages the Digital Credentials within the Wallet Instance, and presents them to Verifiers. The Holder is the User in control of the Wallet.
     - 
   * - Holder Key Binding
     - Ability of the Holder to prove legitimate possession of the private part, related to the public part attested by a Trusted Third Party.
     - 
   * - Identity and Access Management (IAM)
     - Identity and access management, or IAM, is a framework of business processes, policies and technologies that facilitates the management of digital identities. With an IAM framework in place, IT security teams can control user access to critical information within their organizations.
     - 
   * - Key Attestation
     - An attestation from the device's OEM that enhances your confidence in the keys used in your Wallet Instance being securely stored within the device's hardware-backed keystore. Its content is therefore defined by the operating system manufacturer. For Google Android, the term Key Attestation refers to the Strongbox Key Attestation feature. For Apple iOS, the reference is to the `Device Check`_ service, specifically the `attestKey`_ feature.
     - 
   * - Level of Assurance
     - The degree of confidence in the vetting process used to establish the identity of the User and the degree of confidence that the User who presents the credential is the same User to whom the Digital Credential was issued.
     - 
   * - Metadata
     - Digital artifact that contains all the required information about an Organizational Entity, e.g., protocol related endpoints and the Organizational Entity’s cryptographic public keys (for the complete list check requirement “Metadata Content”).
     - 
   * - National Accreditation Bodies (NAB)
     - A body that performs accreditation with authority derived from a Member State under Regulation (EC) No 765/2008.
     - | Alignes with ARF v1.4.
       | 
       | *Alternative terms:*  Accreditation Authority.
   * - National Identity Provider
     - It represents preexisting identity systems based on SAML2 or OpenID Connect Core 1.0, already in production in each Member State (eg: the Italian SPID and CIE id schemes notified eIDAS with *LoA* **High**, see `SPID/CIE-OpenID-Connect-Specifications`_).
     - 
   * - Notification Process
     - Process defining how information is transferred to the European Commission and the inclusion of an entity in the Trusted List.
     - 
   * - Organizational Entity
     - A legal person (only considering organizations and public entities, not natural/physical persons) recognized by the Member State through a unique identifier to operate a certain role within the EUDI Wallet ecosystem.
     - | In this category the following entity roles are included: Wallet Provider, Credential Issuer, Relying Party, QTSP In general, any kind of Entity that must be registered through a national or European registration mechanism.
       | 
       | *Alternative terms:* legal person (only considering organizations and public entities, not natural/physical persons).
   * - PID Provider
     - A Credential Issuer responsible for issuing and revoking Person Identification Data (PID) to Users, ensuring that the PID of a User is cryptographically bound to a Wallet Unit.
     - Notes
   * - Name
     - | Revised from ARF v1.4 and Implementing Act.
       | 
       | *Differences:* editorial (renamed “Member Stare or other legal entity” and "natural or legal person", respectively).
     - 
   * - Policy Language
     - A formal language used to define security, privacy, and identity management policies that govern interactions and transactions within a Trust Framework. This language allows for the clear and unambiguous expression of rules and conditions, facilitating the automation of processes and interoperability among different systems and organizations.
     - 
   * - Primary Actors
     - The set of Public Entities and Private Entities that implement the Technical Solutions for the functioning of the IT-Wallet System.
     - 
   * - Pseudonym
     - Pseudonyms are alternative identifier used to represent an entity (such as a person or organization) without revealing their true identity. It provides a layer of privacy and anonymity while still allowing for consistent authentication and authorization within a system.
     - 
   * - Name
     - Description
     - Notes
   * - Name
     - Description
     - Notes
   * - Name
     - Description
     - Notes
   * - Name
     - Description
     - Notes

Acronyms
--------

.. list-table::
  :widths: 20 80
  :header-rows: 1

  * - **Acronym**
    - **Description**
  * - **OID4VP**
    - OpenID for Verifiable Presentation
  * - **PID**
    - Person Identification Data
  * - **VC**
    - Verifiable Credential
  * - **VP**
    - Verifiable Presentation
  * - **API**
    - Application Programming Interface
  * - **LoA**
    - Level of Assurance
  * - **AAL**
    - Authenticator Assurance Level as defined in `<https://csrc.nist.gov/glossary/term/authenticator_assurance_level>`_
  * - **PII**
    - Personally Identifiable Information
  * - **WSCD**
    - Wallet Secure Cryptographic Device
  * - **WSCA**
    - Wallet Secure Cryptographic Application
  * - **CIE**
    - National Electronic Identity Card
  * - **SPID**
    - Italian Public Digital Identity System
  * - **ANPR**
    - Italian National Registry of the Resident Population

Normative Language and Conventions
--------

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "NOT RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in BCP 14 [RFC2119] [RFC8174] when, and only when, they appear in all capitals, as shown here.
