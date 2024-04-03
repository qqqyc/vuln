# eLearning System –Stored XSS on (Add Subject module) 
# Vendor Homepage:
https://www.sourcecodester.com/php/14787/elearning-system-using-phpmysqli-source-code.html 
Version:V1.0
Tested on: PHP, Apache, MySQL
# Proof of vulnerability:
Log in to the admin system, select Maintenance module, add a new Subject module, and add payload to the Subject code and Description to submit the data.
<img width="416" alt="image" src="https://github.com/qqqyc/vuln/assets/53200267/646dfa36-8c7d-4494-bdef-681f903c3805">

# Payload：
</script><script>alert(1)</script>
# Trigger popup：
As long as visit http://localhost/elearning/admin/?page=subject, it will trigger a pop-up window, the data has been stored in the database.

<img width="416" alt="image" src="https://github.com/qqqyc/vuln/assets/53200267/030160d6-471e-423e-9075-cffc5a6f6d75">
