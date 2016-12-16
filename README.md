# Python Plate Number Verifier
> Nigerian Vehicle Plate Number Verifier

This library enables you verify plate number (of Nigerian vehicles) and get the details
of the vehicle and the verified owner.

## Installation
To use, simply install using pip or easy_install:

> Install the requirements first:

```shell
pip install requests
pip install python-dateutil
```
> And then install number_verifier

```shell
  pip install number_verifier
```


## Example usage:
```python
from number_verifier.NumberOwner import VerifyOwner
vo = VerifyOwner("FST918EH").verify()

issue_date = vo.get_issue_date()
```

#Available details:
After getting an instance of VerifiedOwner (which is what VerifyOwner({number}).verify()) would return, you can do these:

```python
#assuming the object is called 'vo'
from number_verifier.NumberOwner import VerifyOwner
vo = VerifyOwner("FST918EH").verify()
owner = vo.get_owner()
model = vo.get_model()
colour = vo.get_colour()
chasis_number = vo.get_chasis_number()
issue_date = vo.get_issue_date() #This returns a python datetime object
expiry_date = vo.get_expiry_date() #This returns a python datetime object
```



This library is licensed under the <a href="https://github.com/yusufoguntola/number_verifier/blob/master/LICENSE.txt">MIT License.</a> Please take a look at it!

Enjoy!!!
