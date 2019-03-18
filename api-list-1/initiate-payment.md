# Send Token

Used to send/resend a verification token to the user and start the verification session.

**Method:** POST  
**Action:** send-token

## Request

**Format:** POST data

* action `required` : string \(32\)

| Remark | **Sample** |
| :--- | :--- |
| The action of this call, must be hardcoded to “send-token” | send-token |

* timestamp `required` : timestamp \(32\)

| Remark | **Sample** |
| :--- | :--- |
| The timestamp for this API call. | 1539677150 |

* api\_key `required`: string \(32\)

| Remark | **Sample** |
| :--- | :--- |
| Pipwave-assigned merchant’s API key. | sdvdas23t3btg34bhb |

* user\_id `required` : string \(32\)

| Remark | **Sample** |
| :--- | :--- |
| The user ID owning the phone number for verification. | 505315 |

* contact\_no\_country\_dialing\_code `required`: string \(5\)

| Remark | Sample |
| :--- | :--- |
| The country dialing code, without leading symbols. | 60 |

* contact\_no: string \(32\)

| Remark | Sample |
| :--- | :--- |
| The contact number without country dialing code and no symbols / space. | 123456789 |

## Response

**Format:** POST data

{% api-method method="get" host="" path="" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-form-data-parameters %}
{% api-method-parameter name="seconds\_till\_resend" type="integer" required=false %}
If too frequent send/resend request is received, this value will be returned, along with a different status.
{% endapi-method-parameter %}

{% api-method-parameter name="reference" type="integer" required=false %}
The ID of the session, to be echo-ed when calling verify-token-answer API
{% endapi-method-parameter %}

{% api-method-parameter name="message" type="string" required=false %}
Error message, if any
{% endapi-method-parameter %}

{% api-method-parameter name="status" type="string" required=false %}
Status of the request. Refer to appendix for list of possible values.  
  
Sample: 200
{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

## Signature

The data involved in generating the signature for this API are: 

* `timestamp`
* `action`
* `api_key`
* `user_id`
* `contact_no_country_dialing_code`
* `contact_no`

