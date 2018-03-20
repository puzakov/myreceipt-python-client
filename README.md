# swagger-client
Описание взаимодействия с сервисом аренды кассовой техники MyReceipt

This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0
- Package version: 1.0.0
- Build package: io.swagger.codegen.languages.PythonClientCodegen

## Requirements.

Python 2.7 and 3.4+

## Installation & Usage
### pip install

If the python package is hosted on Github, you can install directly from Github

```sh
pip install git+https://github.com//.git
```
(you may need to run `pip` with root permission: `sudo pip install git+https://github.com//.git`)

Then import the package:
```python
import swagger_client 
```

### Setuptools

Install via [Setuptools](http://pypi.python.org/pypi/setuptools).

```sh
python setup.py install --user
```
(or `sudo python setup.py install` to install the package for all users)

Then import the package:
```python
import swagger_client
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: token
swagger_client.configuration.api_key = {'X-Auth-Token': 'YOUR_API_KEY'}
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# swagger_client.configuration.api_key_prefix['X-Auth-Token'] = 'Bearer'
# create an instance of the API class
api_instance = swagger_client.ReceiptApi()
request = swagger_client.ReceiptRequest() # ReceiptRequest | Полная информация о чеке

try:
    # Пробитие чека
    api_response = api_instance.receipt_compose(request)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ReceiptApi->receipt_compose: %s\n" % e)

```

## Documentation for API Endpoints

All URIs are relative to *https://api.myreceipt.tk*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ReceiptApi* | [**receipt_compose**](docs/ReceiptApi.md#receipt_compose) | **POST** /receipt/compose | Пробитие чека
*StatusApi* | [**device_status**](docs/StatusApi.md#device_status) | **GET** /status/device/{id} | Полная информация об устройстве


## Documentation For Models

 - [DeviceStatusResponse](docs/DeviceStatusResponse.md)
 - [Receipt](docs/Receipt.md)
 - [ReceiptClient](docs/ReceiptClient.md)
 - [ReceiptItems](docs/ReceiptItems.md)
 - [ReceiptRequest](docs/ReceiptRequest.md)
 - [ReceiptResponse](docs/ReceiptResponse.md)
 - [Tax](docs/Tax.md)
 - [Taxes](docs/Taxes.md)


## Documentation For Authorization


## token

- **Type**: API key
- **API key parameter name**: X-Auth-Token
- **Location**: HTTP header


## Author


