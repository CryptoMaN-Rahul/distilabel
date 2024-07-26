# AnthropicLLM


Anthropic LLM implementation running the Async API client.







### Attributes

- **model**: the name of the model to use for the LLM e.g. "claude-3-opus-20240229",  "claude-3-sonnet-20240229", etc. Available models can be checked here:  [Anthropic: Models overview](https://docs.anthropic.com/claude/docs/models-overview).

- **api_key**: the API key to authenticate the requests to the Anthropic API. If not provided,  it will be read from `ANTHROPIC_API_KEY` environment variable.

- **base_url**: the base URL to use for the Anthropic API. Defaults to `None` which means  that `https://api.anthropic.com` will be used internally.

- **timeout**: the maximum time in seconds to wait for a response. Defaults to `600.0`.

- **max_retries**: The maximum number of times to retry the request before failing. Defaults  to `6`.

- **http_client**: if provided, an alternative HTTP client to use for calling Anthropic  API. Defaults to `None`.

- **_api_key_env_var**: the name of the environment variable to use for the API key. It  is meant to be used internally.

- **_aclient**: the `AsyncAnthropic` client to use for the Anthropic API. It is meant  to be used internally. Set in the `load` method.





### Runtime Parameters

- **api_key**: the API key to authenticate the requests to the Anthropic API. If not  provided, it will be read from `ANTHROPIC_API_KEY` environment variable.

- **base_url**: the base URL to use for the Anthropic API. Defaults to `"https://api.anthropic.com"`.

- **timeout**: the maximum time in seconds to wait for a response. Defaults to `600.0`.

- **max_retries**: the maximum number of times to retry the request before failing.  Defaults to `6`.




