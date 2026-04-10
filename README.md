
# Getting Started with Fortis API

## Install the Package

The package is compatible with Python versions `3.7+`.
Install the package from PyPi using the following pip command:

```bash
pip install fortis-apimatic-sdk==1.0.3
```

You can also view the package at:
https://pypi.python.org/pypi/fortis-apimatic-sdk/1.0.3

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | [`Environment`](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/README.md#environments) | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| http_client_instance | `Union[Session, HttpClientProvider]` | The Http Client passed from the sdk user for making requests |
| override_http_client_configuration | `bool` | The value which determines to override properties of the passed Http Client from the sdk user |
| http_call_back | `HttpCallBack` | The callback value that is invoked before and after an HTTP call is made to an endpoint |
| timeout | `float` | The value to use for connection timeout. <br> **Default: 60** |
| max_retries | `int` | The number of times to retry an endpoint call if it fails. <br> **Default: 0** |
| backoff_factor | `float` | A backoff factor to apply between attempts after the second try. <br> **Default: 2** |
| retry_statuses | `Array of int` | The http statuses on which retry is to be done. <br> **Default: [408, 413, 429, 500, 502, 503, 504, 521, 522, 524]** |
| retry_methods | `Array of string` | The http methods on which retry is to be done. <br> **Default: ["GET", "PUT"]** |
| proxy_settings | [`ProxySettings`](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/proxy-settings.md) | Optional proxy configuration to route HTTP requests through a proxy server. |
| logging_configuration | [`LoggingConfiguration`](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/logging-configuration.md) | The SDK logging configuration for API calls |
| user_id_credentials | [`UserIdCredentials`](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/auth/custom-header-signature.md) | The credential object for Custom Header Signature |
| user_api_key_credentials | [`UserApiKeyCredentials`](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/auth/custom-header-signature-1.md) | The credential object for Custom Header Signature |
| developer_id_credentials | [`DeveloperIdCredentials`](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/auth/custom-header-signature-2.md) | The credential object for Custom Header Signature |
| access_token_credentials | [`AccessTokenCredentials`](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/auth/custom-header-signature-3.md) | The credential object for Custom Header Signature |

The API client can be initialized as follows:

### Code-Based Client Initialization

```python
import logging

from fortisapi.configuration import Environment
from fortisapi.fortisapi_client import FortisapiClient
from fortisapi.http.auth.access_token import AccessTokenCredentials
from fortisapi.http.auth.developer_id import DeveloperIdCredentials
from fortisapi.http.auth.user_api_key import UserApiKeyCredentials
from fortisapi.http.auth.user_id import UserIdCredentials
from fortisapi.logging.configuration.api_logging_configuration import LoggingConfiguration
from fortisapi.logging.configuration.api_logging_configuration import RequestLoggingConfiguration
from fortisapi.logging.configuration.api_logging_configuration import ResponseLoggingConfiguration

client = FortisapiClient(
    user_id_credentials=UserIdCredentials(
        user_id='user-id'
    ),
    user_api_key_credentials=UserApiKeyCredentials(
        user_api_key='user-api-key'
    ),
    developer_id_credentials=DeveloperIdCredentials(
        developer_id='developer-id'
    ),
    access_token_credentials=AccessTokenCredentials(
        access_token='access-token'
    ),
    environment=Environment.PRODUCTION,
    logging_configuration=LoggingConfiguration(
        log_level=logging.INFO,
        request_logging_config=RequestLoggingConfiguration(
            log_body=True
        ),
        response_logging_config=ResponseLoggingConfiguration(
            log_headers=True
        )
    )
)
```

### Environment-Based Client Initialization

```python
from fortisapi.fortisapi_client import FortisapiClient

# Specify the path to your .env file if it’s located outside the project’s root directory.
client = FortisapiClient.from_environment(dotenv_path='/path/to/.env')
```

See the [Environment-Based Client Initialization](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/environment-based-client-initialization.md) section for details.

## Environments

The SDK can be configured to use a different environment for making API calls. Available environments are:

### Fields

| Name | Description |
|  --- | --- |
| PRODUCTION | **Default** |
| ENVIRONMENT2 | - |

## Authorization

This API uses the following authentication schemes.

* [`user-id (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/auth/custom-header-signature.md)
* [`user-api-key (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/auth/custom-header-signature-1.md)
* [`developer-id (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/auth/custom-header-signature-2.md)
* [`access-token (Custom Header Signature)`](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/auth/custom-header-signature-3.md)

## List of APIs

* [Async Processing](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/async-processing.md)
* [Declined Recurring Transactions](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/declined-recurring-transactions.md)
* [Device Terms](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/device-terms.md)
* [Full Boarding](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/full-boarding.md)
* [3 DS Authentication](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/3-ds-authentication.md)
* [3 DS Transactions](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/3-ds-transactions.md)
* [Merchant Deposits](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/merchant-deposits.md)
* [On Boarding](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/on-boarding.md)
* [Payment Card Reader Token](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/payment-card-reader-token.md)
* [Quick Invoices](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/quick-invoices.md)
* [Transaction ACH Retries](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/transaction-ach-retries.md)
* [Transactions-ACH](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/transactions-ach.md)
* [Transactions-Cash](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/transactions-cash.md)
* [Transactions-Credit Card](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/transactions-credit-card.md)
* [Transactions-EBT Card](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/transactions-ebt-card.md)
* [Transactions-Read](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/transactions-read.md)
* [Level 3 Data](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/level-3-data.md)
* [Transactions-Updates](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/transactions-updates.md)
* [User Verifications](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/user-verifications.md)
* [Apple Pay Validate Merchant](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/apple-pay-validate-merchant.md)
* [Merchant Details](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/merchant-details.md)
* [Batches](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/batches.md)
* [Contacts](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/contacts.md)
* [Elements](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/elements.md)
* [Locations](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/locations.md)
* [Paylinks](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/paylinks.md)
* [Recurring](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/recurring.md)
* [Signatures](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/signatures.md)
* [Tags](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/tags.md)
* [Terminals](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/terminals.md)
* [Tickets](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/tickets.md)
* [Tokens](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/tokens.md)
* [Users](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/users.md)
* [Webhooks](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/controllers/webhooks.md)

## SDK Infrastructure

### Configuration

* [ProxySettings](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/proxy-settings.md)
* [Environment-Based Client Initialization](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/environment-based-client-initialization.md)
* [AbstractLogger](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/abstract-logger.md)
* [LoggingConfiguration](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/logging-configuration.md)
* [RequestLoggingConfiguration](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/request-logging-configuration.md)
* [ResponseLoggingConfiguration](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/response-logging-configuration.md)

### HTTP

* [HttpResponse](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/http-response.md)
* [HttpRequest](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/http-request.md)

### Utilities

* [ApiResponse](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/api-response.md)
* [ApiHelper](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/api-helper.md)
* [HttpDateTime](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/http-date-time.md)
* [RFC3339DateTime](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/rfc3339-date-time.md)
* [UnixDateTime](https://www.github.com/sdks-io/fortis-apimatic-python-sdk/tree/1.0.3/doc/unix-date-time.md)

