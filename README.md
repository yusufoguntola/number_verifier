Nigerian Vehicle Plate Number Verifier

This library enables you verify plate number (of Nigerian vehicles) and get the details
of the vehicle and the verified owner.

To use, simply install using pip or easy_install:

Type:
<code>pip install number_verifier</code>

or

<code>easy_install install number_verifier</code>

Example usage:
<code>from number_verifier.NumberOwner import VerifyOwner</code>

<code>vo = VerifyOwner("FST918EH").verify()</code>

<code>issue_date = vo.get_issue_date()</code>

Available details:
After getting an instance of VerifiedOwner (which is what VerifyOwner({number}).verify()) would return, you can do these:

<code>#assuming the object is called 'vo'</code>

<code>owner = vo.get_owner()</code>
  
<code>model = vo.get_model()</code>
  
<code>colour = vo.get_colour()</code>
  
<code>chasis_number = vo.get_chasis_number()</code>
  
<code>issue_date = vo.get_issue_date()</code>
  
<code>expiry_date = vo.get_expiry_date()</code>
  



This library is licensed under the <a href="https://github.com/yusufoguntola/number_verifier/blob/master/LICENSE.txt">MIT License.</a> Please take a look at it!

Enjoy!!!
