# Errors
A description of all errors developers might face when integrating with one of SP's clients.

## SDKs

### Common to iOS and Android

|Name|Description|Code|
|----|-----------|----|
|InvalidResponseWebMessage|when the response from getting the message is invalid|sp_metric_invalid_response_web_message|
|InvalidResponseNativeMessage|when the response from getting the native message is invalid|sp_metric_invalid_response_native_message|
|InvalidResponseConsent|when the response from posting consent is invalid|sp_metric_invalid_response_consent|
|InvalidResponseCustomConsent|when the response from posting custom consent is invalid|sp_metric_invalid_response_custom_consent|
|InvalidEventPayload|the event payload coming from the webview is invalid|sp_metric_invalid_event_payload|
|InvalidOnActionEventPayload|event payloads are not expected onAction|sp_metric_invalid_onAction_event_payload|
|InvalidRequestError|When the SDK doesn't have all the necessary data to perform a request.|sp_metric_invalid_request_error|
|RenderingApp|JS on error is called|_multiple_|
|WebView|WebView error handler|sp_metric_web_view_error|
|NoInternetConnection|User has no Internet connection.|sp_metric_no_internet_connection|
|InternalServer|5xx|sp_metric_internal_server_error_5xx|
|ResourceNotFound|4xx|sp_metric_resource_not_found_4xx|
|ConnectionTimeout|Timed out when loading {url} after {x} seconds.|sp_metric_connection_timeout|
|GenericNetworkRequest|Generic network request error|sp_metric_generic_network_request|

### iOS Specific

|Name|Description|Code|
|----|-----------|----|
|InvalidURL|When an URL cannot be constructed|sp_metric_invalid_url|
|UnableToLoadJSReceiver|The SDK wasn't able to load (or inject) the Javascript intercace into the webview|sp_metric_unable_to_load_jsreceiver|

### Android Specific

|Name|Description|Code|
|----|-----------|----|
|GenericSDKException|Catch all exception|sp_metric_generic_sdk_error|
|InvalidLocalDataException|a property is missing from local storage or in a configuration object|sp_metric_invalid_local_data|
