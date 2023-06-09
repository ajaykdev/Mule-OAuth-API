# MuleSoft OAuth Project POC

This project is a proof-of-concept (POC) implementation of OAuth in MuleSoft. OAuth is an industry-standard authorization protocol that allows third-party applications to access protected resources on behalf of the resource owner. 

The purpose of this project is to demonstrate how to implement OAuth in MuleSoft, using the Anypoint Platform and the OAuth 2.0 Authorization Framework. The project includes the necessary configurations to create an OAuth provider and an OAuth client, and to secure MuleSoft APIs using OAuth.

## Requirements

To run this project, you will need:

- Anypoint Studio 7.5 or later
- Mule Runtime 4.3 or later
- Anypoint Platform account
- OAuth 2.0 client credentials (client ID and client secret)

## Installation

1. Clone this repository to your local machine.
2. Import the project into Anypoint Studio.
3. Update the `client_id` and `client_secret` properties in the `oauth-configuration.xml` file with your OAuth client credentials.
4. Deploy the project to your MuleSoft runtime.

## Usage

Once the project is deployed, you can use the following endpoints to test the OAuth implementation:

- `http://localhost:8081/createclient` - this endpoint is for generating clientId and clientSecret for the client.
- `http://localhost:8081/token` - this endpoint is for generating oAuth token for the given client.
- `http://localhost:8081/validate` - this endpoint is for validating the client with provided oAuth token.


To obtain an OAuth access token, you can use the OAuth client credentials grant type. This project includes a sample client credentials flow that you can use to obtain an access token. You can find this flow in the `client-credentials-grant.xml` file.


## Contributing

Contributions to this project are welcome. If you find a bug or want to suggest an enhancement, please open an issue or submit a pull request.


