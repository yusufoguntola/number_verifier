Nigerian Vehicle Plate Number Verifier

This library enables you verify plate number (of Nigerian vehicles) ang get the details
of the vehicle and the verified owner.

To use, simply install using pip or easy_install:

Type:
<code>pip install number_verifier</code>
or
<code>easy_install install number_verifier</code>

Example usage:

<code>vo = VerifyOwner("FST918EH").verify()</code>
<code>issue_date = vo.get_issue_date()</code>

Available details:
After getting an instance of VerifiedOwner (which is what VerifyOwner({number}).verify()) would return, you can do these:
<code>#assuming the object is called 'vo'</code>
<code>
  owner = vo.get_owner()
  model = vo.get_model()
  colour = vo.get_colour()
  chasis_number = vo.get_chasis_number()
  issue_date = vo.get_issue_date()
  expiry_date = vo.get_expiry_date()
</code>


This library is licensed under the MIT License. Please take a look at it!

Enjoy!!!
