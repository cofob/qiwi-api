# qiwi-api
Python QIWI payments API

## Quick Example
```python
import qiwi


def callback(tx: qiwi.types.Transaction):
    print('New transaction!', tx.account, tx.amount, tx.comment)


qiwi_api = qiwi.Qiwi('a4xxxxxxxxxxxxxxxxxxxxxee', '7xxxxxxxxx3', callback=callback)
qiwi_api.start()
```
