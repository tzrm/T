Isolation level: Serializable

- statements cannot read data that has been modified but not yet commited by other transactions
- no other transactions can modify data that has been read by the current transaction unitl the current transaction completes
- other transactions cannot insert new rows with key values that would fall in the range of keys read by any statements in the current transaction until the current transaction completes