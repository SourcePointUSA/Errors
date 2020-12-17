# Errors
A description of all errors developers might face when integrating with one of SP's clients.

## SDKs

### Common to iOS and Android

|Name|Description|Code|
|----|-----------|----|
|InvalidResponseWebMessage|when the response from getting the message is invalid|invalid_response_web_message|
|InvalidResponseNativeMessage|when the response from getting the native message is invalid|invalid_response_native_message|
|InvalidResponseConsent|when the response from posting consent is invalid|invalid_response_consent|
|InvalidResponseCustomConsent|when the response from posting custom consent is invalid|invalid_response_custom_consent|
|InvalidEventPayload|the event payload coming from the webview is invalid|invalid_event_payload|
|InvalidOnActionEventPayload|event payloads are not expected onAction|invalid_onAction_event_payload|
|InvalidRequestError|When the SDK doesn't have all the necessary data to perform a request.|invalid_request_error|
|RenderingApp|JS on error is called|_multiple_|
|WebView|WebView error handler|web_view_error|
|NoInternetConnection|User has no Internet connection.|no_internet_connection|
|InternalServer|5xx|internal_server_error_5xx|
|ResourceNotFound|4xx|resource_not_found_4xx|
|ConnectionTimeout|Timed out when loading {url} after {x} seconds.|connection_timeout|
|GenericNetworkRequest|Generic network request error|generic_network_request|

### iOS Specific

|Name|Description|Code|
|----|-----------|----|
|InvalidURL|When an URL cannot be constructed|invalid_url|
|UnableToLoadJSReceiver|The SDK wasn't able to load (or inject) the Javascript intercace into the webview|unable_to_load_jsreceiver|

### Android Specific

|Name|Description|Code|
|----|-----------|----|
|GenericSDKException|Catch all exception|generic_sdk_error|
|InvalidLocalDataException|a property is missing from local storage or in a configuration object|invalid_local_data|
