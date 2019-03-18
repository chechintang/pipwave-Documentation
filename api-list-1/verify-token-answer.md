# Verify Token Answer

Used to verify the answer provided by the user.

**Method:** POST  
**Action:** verify-token-answer

## Request

**Format:** POST data

* action `required`: string \(32\)

| Remarks | Sample |
| :--- | :--- |
| The action of this call, must be hardcoded to “verify-token-answer” | verify-token-answer |

* timestamp `required`: timestamp \(32\)

| Remarks | Sample |
| :--- | :--- |
| The timestamp for this API call. | 1539677150 |

* api\_key `required`: string \(32\)

| Remarks | Sample |
| :--- | :--- |
| Pipwave-assigned merchant’s API key. | sdvdas23t3btg34bhb |

* user\_id `required`: string \(32\)

| Remarks | Sample |
| :--- | :--- |
| The user ID owning the phone number for verification. | 505315 |

* reference: integer

| Remarks | Sample |
| :--- | :--- |
| The reference ID returned by send-token API. | 164 |

* contact\_no\_country\_dialing\_code `required`: string \(5\)

| Remarks | Sample |
| :--- | :--- |
| The country dialing code, without leading symbols. | 60 |

* contact\_no: string \(32\)

| Remarks | Sample |
| :--- | :--- |
| The contact number without country dialing code and no symbols / space. | 123456789 |

* answer: string \(6\)

| Remarks | Sample |
| :--- | :--- |
| The answer. | 123456 |

## Response

**Format:** JSON

* status: string \(5\)

| Remarks | Sample |
| :--- | :--- |
| Status of the request. Refer to appendix for list of possible values. | 200 |

* message: string \(255\)

| Remarks | Sample |
| :--- | :--- |
| Error message, if any | - |

## Signature

The data involved in generating the signature for this API are: 

* timestamp
* action
* api\_key user\_id
* reference
* contact\_no\_country\_dialing\_code
* contact\_no
* answer

