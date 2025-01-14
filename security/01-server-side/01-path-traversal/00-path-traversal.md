# Path traversal

Directory traversal vulnerabilities enable an attacker to read arbitrary files
on the server that is running an application.

This might include:
- Application code and data
- Credentials for back-end systems
- Sensitive operating system files

<!-- Resources {{{-->
## Resources

- [CVE-XXXX-XXXX](https://www.example.com/)

<!-- }}} -->

<!-- Description {{{-->
## Description



<!-- }}} -->

<!-- Impact {{{-->
## Impact



<!-- }}} -->

<!-- Exploitation {{{-->
## Exploitation

This application implements no defenses against path traversal attacks
```html
<img src="/loadImage?filename=218.png">
```

An attacker can request the following URL to retrieve a file
```
https://insecure-website.com/loadImage?filename=../../../etc/passwd
```

This causes the application to read from the following path
```sh
/var/www/images/../../../etc/passwd
```

<!-- }}} -->

<!-- Remediation {{{-->
## Remediation



<!-- }}} -->
