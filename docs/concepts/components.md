# Open DID Architecture
This document explains the main components that make up the Open DID system and provides an overall architecture diagram.

## Open DID Components
The components of the Open DID system include entities, services, and providers. Providers combine entities to offer services. The diagram below shows how these components are structured.

![overview](../../assets/components.png)

### Entities
Entities perform a single function. Each entity has a specific role, and the main entities in Open DID are as follows:
* **TA (Trusted Authority)**: Responsible for registering all providers into the Open DID system to establish trust relationships.
* **Issuer**: Holds the user's identity or qualification information and issues digital IDs to the users.
* **Verifier**: Requests and verifies the user's digital ID to provide services.

### Services
Services combine the functions of various entities into products. Services can be offered in various forms such as servers, apps, or SDKs. Examples of services include:
* **Digital ID Issuance and Management Service**
    * **Entities**: Issuer, Wallet, Notification
    * **Description**: A service that issues and manages digital IDs for users. The Issuer entity issues and renews digital IDs based on user identity information, the Wallet entity securely stores and manages issued digital IDs, and the Notification entity supports sending notifications related to ID issuance and renewal.

* **Notification and Log Management Service**
    * **Entities**: Notification, Log, Storage
    * **Description**: Manages notifications related to events occurring within the system and collects and stores all log data to provide necessary statistical data. The Notification entity sends notifications in a user-defined manner, the Log entity records and stores event logs, and the Storage entity securely stores and manages this data.

* **Integrated Security and Authentication Service**
    * **Entities**: KYC, OP
    * **Description**: Provides services for user authentication and authorization management. The KYC entity verifies and authenticates the user's identity, while the OP entity issues secure tokens based on the authenticated information and grants permissions to users.

### Providers
Providers are entities that combine various services to offer comprehensive solutions.

## Overall Architecture
The diagram below represents the overall architecture of Open DID. To clearly illustrate the entities that make up Open DID, each provider is assumed to offer a single service, and that service provides the function of a single entity.

![components_overview](../../assets/components_overview.png)