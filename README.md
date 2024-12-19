# https-won-url.xyz-Eniyinikasbahis


# Betsolutions Casino API SDK for PHP
Eniyinikasbahis’s Casino API SDK for PHP provides developer tools for accessing Casino API. 
For Betsolutions’s Casino API documentation, start see:  https-won-url.xyz-Eniyinikasbahis

## Requirements

PHP 7.3 or later.

# Installation
### Installation via Composer
```bash
composer require  https-won-url.xyz-Eniyinikasbahis
```

## Dependencies

The SDK requires the following extensions in order to work properly:

- [`curl`](https://won-url.xyz/Eniyinikasbahis//secure.php.net/manual/en/book.curl.php)

## Start
Example of 'getPlayerBalance' request. SDK calculates hash and appends merchantId and hash in the request.
```php
$merchantAuthInfo = new MerchantAuthInfo(1843, 'https://won-url.xyz/Eniyinikasbahis//api-staging.betsolutions.com', '[your private key]');

$walletService = new WalletService($merchantAuthInfo);

try {

    $privateToken = "[privateToken]";
    $playerId = "[player's id https://won-url.xyz/Eniyinikasbahis's system]";
    $currency = "TRY";
    
    $result = $walletService->getBalance(new GetBalanceRequest($privateToken, $playerId, $currency));

    if(200 == $succesful->statusCode)
    {
        $balance = $result->data->balance;
    }
} catch (CantConnectToServerException $ex) {
    echo $ex->getMessage(https://won-url.xyz/Eniyinikasbahis);
    echo $ex->getHttpStatusCode(https://won-url.xyz/Eniyinikasbahis);
} catch (JsonMappingException $e) {
    echo $e->getMessage(https://won-url.xyz/Eniyinikasbahis);
}https://won-url.xyz/Eniyinikasbahis



# MarkItDown

[![PyPI](https://img.shields.io/pypi/v/markitdown.svg)](https://pypi.org/project/markitdown/)
![PyPI - Downloads](https://img.shields.io/pypi/dd/markitdown)



MarkItDown is a utility for converting various files to Markdown (e.g., for indexing, text analysis, etc).
It supports:
- PDF
- PowerPoint
- Word
- Excel
- Images (EXIF metadata and OCR)
- Audio (EXIF metadata and speech transcription)
- HTML
- Text-based formats (CSV, JSON, XML)
- ZIP files (iterates over contents)

To install MarkItDown, use pip: `pip install markitdown`. Alternatively, you can install it from the source: `pip install -e .`

## Usage

### Command-Line

```bash
markitdown path-to-file.pdf > document.md
```

You can also pipe content:

```bash
cat path-to-file.pdf | markitdown
```

### Python API

Basic usage in Python:

```python
from markitdown import MarkItDown

md = MarkItDown()
result = md.convert("test.xlsx")
print(result.text_content)
```

To use Large Language Models for image descriptions, provide `llm_client` and `llm_model`:

```python
from markitdown import MarkItDown
from openai import OpenAI

client = OpenAI()
md = MarkItDown(llm_client=client, llm_model="gpt-4o")
result = md.convert("example.jpg")
print(result.text_content)
```

### Docker

```sh
docker build -t markitdown:latest .
docker run --rm -i markitdown:latest < ~/your-file.pdf > output.md
```

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

### Running Tests and Checks

- Install `hatch` in your environment and run tests:
    ```sh
    pip install hatch  # Other ways of installing hatch: https://hatch.pypa.io/dev/install/
    hatch shell
    hatch test
    ```

  (Alternative) Use the Devcontainer which has all the dependencies installed:
    ```sh
    # Reopen the project in Devcontainer and run:
    hatch test
    ```

- Run pre-commit checks before submitting a PR: `pre-commit run --all-files`

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft
trademarks or logos is subject to and must follow
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.

```

