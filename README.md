# Getting Started With Hashicorp Vault

https://www.youtube.com/watch?v=b_2lo30g0RU


Welcome to my github repo for getting started with Hashicorp Vault. 

Here you can find all of the necessary templates and step by step instructions in order ot set up Hashicorp Vault if you are learning or wanting to try it out.

Feel free to check out the following sections. They'll be updated as I add more content to my video tutorials.

## Tutorials

1. [Setting up Consul & Hashicorp Vault](01-getting-started/)

    We'll walk through the basic set-up of your Vault Server. In this tutorial, we use an Ubuntu 20.04 T.2 Micro instance on AWS.

    - [Install Consul Backend](01-getting-started#installing-consul-backend)
    - [Creating A Cert For The Server](https://github.com/b1tsized/vault-tutorial/tree/main/01-getting-started#creating-a-cert-for-the-server)
    - [Install Hashicorp Vault](01-getting-started#install-hashicorp-vault)

    - [Youtube Tutorial Pt. 1](https://youtu.be/b_2lo30g0RU)
    - [Sys File Templates](01-getting-started/sys_file_templates)
        + [Consul Service File](01-getting-started/sys_file_templates/consul.service)
        + [Consul UI JSON](01-getting-started/sys_file_templates/ui.json)
        + [Vault Config File](01-getting-started/sys_file_templates/config.hcl)
        + [Vault Service File](01-getting-started/sys_file_templates/vault.service)

2. [Creating & Accessing Secrets](02-creating-and-accessing-secrets)

    In this section, we'll go over creation of secrets and accessing them via CLI, Web Interface, or API. 

    - [Enabling The Secret Store Using The CLI](02-creating-and-accessing-secrets#enabling-your-secret-store-using-cli)
    - [Enabling Secrets Using The UI](02-creating-and-accessing-secrets#enabling-secrets-via-the-ui)
    - [Accessing Secrets From a Remote Machine](02-reating-and-accessing-secrets#accessing-secrets-from-a-remote-machine)

    - [Youtube Tutorial Pt. 2](https://youtu.be/LEpk376fc-U)
    - [Payload Template](02-creating-and-accessing-secrets/template/payload.json)

3. [Creating PKI & Enabling Cert Auth](03-creating-pki-and-enabling-cert-auth)

    We'll introduce you to making Vault a certificate authority, creating certificates, importing certificates, and enabling cert auth. We also touch on policies a bit to show how to restrict access or allow access to secrets.

    - [Creating New Secrets](03-creating-pki-and-enabling-cert-auth#creating-new-secrets)
    - [Enabling PKI And Generating Certs](03-creating-pki-and-enabling-cert-auth#enabling-pki-generating-certs-and-signing-them-through-the-cli)
    - [Enable Cert Auth And Adding a Policy](03-creating-pki-and-enabling-cert-auth#enable-cert-auth-and-attaching-a-policy)

    - [Youtube Tutorial Pt. 3](https://youtu.be/_Nqx0guy5RY)
    - [Vault Cert Policy Template](03-creating-pki-and-enabling-cert-auth/template/vault-cert.hcl)

4. [Alternate Auth Methods And SSH Secrets](04-alternate-auth-methods-and-ssh-secrets)

    Here we'll go over other auth methods and introduce you to ssh using Vault.

    - [Enabling Github As An Auth Method](04-alternate-auth-methods-and-ssh-secrets#enabling-github-as-an-auth-method)
    - [Enabling Username and Password Auth Method](04-alternate-auth-methods-and-ssh-secrets#enabling-username--password-for-auth-method)
    - [Adding SSH As A Secret](04-alternate-auth-methods-and-ssh-secrets#adding-ssh-as-a-secret)

    - [YouTube Tutorial Pt. 4](https://youtu.be/R3BzNcJk8YQ)
    - [Sys File Templates](04-alternate-auth-methods-and-ssh-secrets/template/)
        + [SSH Helper Service Config](04-alternate-auth-methods-and-ssh-secrets/template/config.hcl)
        + [OTP Policy](04-alternate-auth-methods-and-ssh-secrets/template/otp-policy.hcl)
        + [Config File](04-alternate-auth-methods-and-ssh-secrets/template/config.hcl)

5. [AWS/GCP Secrets And OKTA SSO](05-aws-gcp-secrets-and-okta-sso)

    We'll be adding in AWS and GCP to be able to generate access credentials for users through Vault rather than through the respective platforms. We'll also set up Vault to us OKTA SSO for authentication.

    - [Enabling AWS IAM Role As A Secret](05-aws-gcp-secrets-and-okta-sso#enabling-aws-iam-role-as-a-secret)
    - [Enabling GCP As A Secret](05-aws-gcp-secrets-and-okta-sso#enabling-gcp-as-a-secret)
    - [Using Okta SSO With Vault](05-aws-gcp-secrets-and-okta-sso#using-okta-sso-with-vault)

    - [Sys File Templates](05-aws-gcp-secrets-and-okta-sso/template)
        + [AWS IAM Policy](05-aws-gcp-secrets-and-okta-sso/template/aws-iam.json)
