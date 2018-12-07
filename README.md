# Expected number of transactions

Beside the transactions that we express through implementation, the Open Contracting Data Standard doesn't provide information for the total number of the expected transactions.

This extension introduces one field that can be used to provide the total number of the expected transactions based on the contract.

## Additional fields

The field introduced by this extensions is:

* ``` contracts/expectedNumberOfTransactions ``` - The expected number of transactions based on the contract

## Example

Simple example: 

```
{
    "ocid": "ocds-213czf-000-00001",
    "id": "ocds-213czf-000-00001-07-close",
    "date": "2012-01-10T09:30:00Z",
    "initiationType": "tender",
    "tag": [
      "contract"
    ],
    "parties": ["..."],
    "buyer": {
      "id": "EU-LAC-E09000003"
    },
    "awards": ["..."],
    "contracts": [
      {
        "id": "ocds-213czf-000-00001-contract-01",
        "awardID": "ocds-213czf-000-00001-award-01",
        "title": "Contract to build new cycle lanes in the centre of town.",
        "period": {
          "startDate": "2010-07-01T00:00:00Z",
          "endDate": "2012-01-01T23:59:00Z",
          "maxExtentDate": "2012-01-31T23:59:00Z"
        },
        "value": {
          "amount": 11500000,
          "currency": "EUR"
        },
        "expectedNumberOfTransactions": 5
      }
    ]
}
```