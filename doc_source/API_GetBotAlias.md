# GetBotAlias<a name="API_GetBotAlias"></a>

Returns information about an Amazon Lex bot alias\. For more information about aliases, see [Versioning and Aliases](versioning-aliases.md)\.

This operation requires permissions for the `lex:GetBotAlias` action\.

## Request Syntax<a name="API_GetBotAlias_RequestSyntax"></a>

```
GET /bots/botName/aliases/name HTTP/1.1
```

## URI Request Parameters<a name="API_GetBotAlias_RequestParameters"></a>

The request requires the following URI parameters\.

 ** botName **   
The name of the bot\.  
Length Constraints: Minimum length of 2\. Maximum length of 50\.  
Pattern: `^([A-Za-z]_?)+$` 

 ** name **   
The name of the bot alias\. The name is case sensitive\.  
Length Constraints: Minimum length of 1\. Maximum length of 100\.  
Pattern: `^([A-Za-z]_?)+$` 

## Request Body<a name="API_GetBotAlias_RequestBody"></a>

The request does not have a request body\.

## Response Syntax<a name="API_GetBotAlias_ResponseSyntax"></a>

```
HTTP/1.1 200
Content-type: application/json

{
   "botName": "string",
   "botVersion": "string",
   "checksum": "string",
   "createdDate": number,
   "description": "string",
   "lastUpdatedDate": number,
   "name": "string"
}
```

## Response Elements<a name="API_GetBotAlias_ResponseElements"></a>

If the action is successful, the service sends back an HTTP 200 response\.

The following data is returned in JSON format by the service\.

 ** botName **   
The name of the bot that the alias points to\.  
Type: String  
Length Constraints: Minimum length of 2\. Maximum length of 50\.  
Pattern: `^([A-Za-z]_?)+$` 

 ** botVersion **   
The version of the bot that the alias points to\.  
Type: String  
Length Constraints: Minimum length of 1\. Maximum length of 64\.  
Pattern: `\$LATEST|[0-9]+` 

 ** checksum **   
Checksum of the bot alias\.  
Type: String

 ** createdDate **   
The date that the bot alias was created\.  
Type: Timestamp

 ** description **   
A description of the bot alias\.  
Type: String  
Length Constraints: Minimum length of 0\. Maximum length of 200\.

 ** lastUpdatedDate **   
The date that the bot alias was updated\. When you create a resource, the creation date and the last updated date are the same\.  
Type: Timestamp

 ** name **   
The name of the bot alias\.  
Type: String  
Length Constraints: Minimum length of 1\. Maximum length of 100\.  
Pattern: `^([A-Za-z]_?)+$` 

## Errors<a name="API_GetBotAlias_Errors"></a>

 **BadRequestException**   
The request is not well formed\. For example, a value is invalid or a required field is missing\. Check the field values, and try again\.  
HTTP Status Code: 400

 **InternalFailureException**   
An internal Amazon Lex error occurred\. Try your request again\.  
HTTP Status Code: 500

 **LimitExceededException**   
The request exceeded a limit\. Try your request again\.  
HTTP Status Code: 429

 **NotFoundException**   
The resource specified in the request was not found\. Check the resource and try again\.  
HTTP Status Code: 404

## See Also<a name="API_GetBotAlias_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:

+  [AWS Command Line Interface](http://docs.aws.amazon.com/goto/aws-cli/lex-models-2017-04-19/GetBotAlias) 

+  [AWS SDK for \.NET](http://docs.aws.amazon.com/goto/DotNetSDKV3/lex-models-2017-04-19/GetBotAlias) 

+  [AWS SDK for C\+\+](http://docs.aws.amazon.com/goto/SdkForCpp/lex-models-2017-04-19/GetBotAlias) 

+  [AWS SDK for Go](http://docs.aws.amazon.com/goto/SdkForGoV1/lex-models-2017-04-19/GetBotAlias) 

+  [AWS SDK for Java](http://docs.aws.amazon.com/goto/SdkForJava/lex-models-2017-04-19/GetBotAlias) 

+  [AWS SDK for JavaScript](http://docs.aws.amazon.com/goto/AWSJavaScriptSDK/lex-models-2017-04-19/GetBotAlias) 

+  [AWS SDK for PHP V3](http://docs.aws.amazon.com/goto/SdkForPHPV3/lex-models-2017-04-19/GetBotAlias) 

+  [AWS SDK for Python](http://docs.aws.amazon.com/goto/boto3/lex-models-2017-04-19/GetBotAlias) 

+  [AWS SDK for Ruby V2](http://docs.aws.amazon.com/goto/SdkForRubyV2/lex-models-2017-04-19/GetBotAlias) 