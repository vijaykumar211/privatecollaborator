# Burp suite private collaborator
A script for installing private Burp Collaborator with Let's Encrypt SSL-certificate.
Should work on (Ubuntu 18.04):
- Amazon AWS EC2 VM with or without Elastic IP.
- DigitalOcean VM with or without Floating IP.
- Any other platform as long as the VM has public IP.

Please see [this blog post](https://teamrot.fi/2019/05/23/self-hosted-burp-collaborator-with-custom-domain/) for usage instructions.

## TL;DR:

make following settings in cloudflare 

![cf](https://raw.githubusercontent.com/vijaykumar211/privatecollaborator/master/burpcollab.png)

1. Clone this repository.
2. Run `sudo ./install.sh your.domain.fi`.
3. You should now have Let's encrypt certificate for the domain and a private burp collaborator properly set up.
4. Start the collaborator with `sudo service burpcollaborator start`.
