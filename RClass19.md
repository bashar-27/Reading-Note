## Itro to Claims

Claims are assertions about a user's identity, attributes, or permissions in an authentication context.
These assertions provide contextual information such as roles, group memberships, and access rights.
Claims-based authentication leverages these attributes to make access control decisions,
enabling more flexible and dynamic authorization processes. This approach enhances security,
enables single sign-on across applications, and simplifies user management by centralizing identity information.

<hr>

## Claims-Based auth

Claims-based authentication is an identity verification approach where a user's attributes,
known as claims, are used to grant or deny access to resources. It allows for more flexible and granular access control,
enabling applications to make informed decisions based on a user's roles, permissions, and other attributes.
Claims-based authentication often involves the use of security tokens that contain these claims and can be easily shared across different applications and services. 
This approach enhances security, simplifies user management, and supports scenarios like single sign-on and federation.

<hr>

## JWT Authentication

JSON Web Token (JWT) authentication is a popular approach used to establish secure communication between a client and a server in various applications, including web and mobile. It addresses the challenges of transmitting sensitive information over an open network while ensuring data integrity and authentication.

Here's a more detailed breakdown of JWT authentication:

Token Structure: JWT is a compact and self-contained token format that consists of three parts separated by dots: header, payload, and signature. The header typically contains metadata about the token, the payload carries the claims (user attributes, roles, etc.), and the signature ensures the token's integrity.

Encoding Claims: Claims are pieces of information that provide context about the user. These can include user ID, roles, permissions, email, and more. The claims are encoded into the token's payload using JSON format, allowing for easy representation and transmission.

Digital Signature: To prevent tampering and unauthorized modifications, the token is digitally signed using a secret key known only to the server. This signature ensures that the token's contents remain unchanged during transmission. Verification of the signature guarantees the authenticity of the token.

Stateless and Efficient: One significant advantage of JWT is its statelessness. Since all the necessary information is embedded within the token itself, the server does not need to maintain session state or query databases to validate the token. This leads to faster and more efficient authentication processes.

Token Exchange: After a user successfully logs in, the server generates a JWT and sends it to the client. Subsequent requests from the client include the JWT in the Authorization header. The server then validates the token's signature, ensuring the user's identity and claims before granting access.
