# Verify Token Answer

Used to verify the answer provided by the user.

**Method:** POST  
**Action:** verify-token-answer

## Request

**Format:** POST data

## Response

**Format:** JSON

## Signature

The data involved in generating the signature for this API are: 

* timestamp
* action
* api\_key user\_id
* reference
* contact\_no\_country\_dialing\_code
* contact\_no answer

