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

* `timestamp`
* `action`
* `api_key user_id`
* `reference`
* `contact_no_country_dialing_code`
* `contact_no answer`

