# Send Token

Used to send/resend a verification token to the user and start the verification session.

**Method:** POST  
**Action:** send-token

## Request

**Format:** POST data

* action **`required`** : string \(32\)

| Remark |  **Sample** |
| :--- | :--- |
| The action of this call, must be hardcoded to “send-token” | send-token |

---

* timestamp **`required`** : timestamp \(32\)

| Remark | **Sample** |
| :--- | :--- |
| The timestamp for this API call. | 1539677150 |

## Response

## Signature

