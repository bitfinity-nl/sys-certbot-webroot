# sys-certbot-webroot
Certbot is a free, open source software tool for automatically using Let’s Encrypt certificates on manually-administrated websites to enable HTTPS.

Example Playbook
----------------

    - hosts: webservers
      become: true

      vars:

        # -- letsencrypt Apache2 settings --
        le_email             : '{{ def_smtp_mail }}'
        le_domain            : 'www.example.nl'

      roles:
         - sys-certbot-webroot

License
-------

GPLv3

Author Information
------------------

E: info@bitfinity.nl

I: https://www.bitfinity.nl
