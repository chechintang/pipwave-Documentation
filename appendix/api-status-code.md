# API Status Code

| API Code | Reason |
| :--- | :--- |
| 200 | OK - For send-token API, it means sending/resending successful, for verify-token-answer API, it means the answer is correct |
| 400 | Failed to fulfill request, see message |
| 401 | Invalid API signature |
| 403 | Invalid API key |
| 404 | Invalid action |
| 500 | Generic server error, see message |
| 5001 | Invalid phone number |
| 5002 | Too frequent request, seconds\_till\_resend will be included in package |
| 5003 | Duplicate verification request for the same contact number |
| 5004 | Insufficient credit |
| 5005 | Solution has been disabled, please contact the administrator |
| 5006 | Merchant has disabled the solution, please enable it at Merchant Portal |
| 5051 | Session has expired or reference not found, please try again |
| 5052 | Incorrect answer provided |
| 9001 | Parameter error, see message |

