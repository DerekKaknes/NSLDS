#Installation
Use '''pip install NSLDS'''

#Usage
Provide NSLDS with your login credentials for the NSLDS site and it will return
the contents of the downloadable text file with all of your loan data.

##Example Usage

```python
from nslds import NSLDS

borrower = NSLDS(borrower_ssn='123456789',
                 borrower_name='NA',
                 borrower_dob='09211990',
                 pin='1234')

loan_data = borrower.get_loan_data()
```

This will store the contents of the downloadable textfile in `loan_data`, which
can then be parsed and processed further.
