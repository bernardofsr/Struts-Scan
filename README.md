##Modified project of: https://github.com/Lucifer1993/struts-scan
[Modification] Work on Python3 
[Modification] Translated to English

# struts-scan
Quickly detect vulnerabilities in struts command execution, and can be batched.

# Operating environment
Python3 under MAC/Linux

#Usage
python3 struts-scan.py "http://example.com"
or
python3 struts-scan.py "http://example.com/anyaction.action"

# Support the detection of the following versions

ST2-005

ST2-008

ST2-009

ST2-013

ST2-016

ST2-019

ST2-020

ST2-devmode

ST2-032

ST2-033

ST2-037

ST2-045

ST2-046

ST2-048

ST2-052

ST2-053

ST2-057

# increase
[+] Shell command interaction for each version

[+]struts2-052 detection (will be added after the use)

[+]struts2-053 detection + utilization (need to provide parameters)

[+] Reasons for output timeout during detection

[+] Compatible with HTTP/1.0, fixed the problem of inaccurate detection of struts-045

[+]struts2-046 detection + utilization

[+]Modify the payload of struts2-048

[+] For some timeout situations, comment out the httplib.HTTPConnection._http_vsn = 10 and httplib.HTTPConnection._http_vsn_str ='HTTP/1.0' two lines and test again, because some may not support the HTTP/1.0 protocol.

[+] Add executable files for linux and win, windows needs .NET environment.

[+] Added the function of writing files, the success.txt file will be automatically written for the struts version number with vulnerabilities.

[+] Increase the detection and utilization of struts2-057, the production environment has not yet found a usable example, it is a tasteless hole, refer to https://github.com/Ivan1ee/struts2-057-exp

# Special Note
This tool is limited to vulnerability verification. If the user causes related legal liabilities, please take your own responsibility, and the developer does not assume joint and several liabilities.
