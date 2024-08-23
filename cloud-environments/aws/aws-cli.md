# AWS CLI 

## Installation

```bash
ZIPNAME=awscliv2.zip
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "$ZIPNAME"
unzip awscliv2.zip
sudo ./aws/install
rm -rf ./aws
rm -rf $ZIPNAME
```

## Configuration

```bash
aws configure sso
SSO session name (Recommended): oa-govcloud
SSO start URL [None]: https://start.us-gov-home.awsapps.com/directory/outsideanalytics
SSO region [None]: us-gov-west-1
SSO registration scopes [sso:account:access]:
Attempting to automatically open the SSO authorization page in your default browser.
If the browser does not open or you wish to use a different device to authorize this request, open the following URL:

https://device.sso.us-gov-west-1.amazonaws.com/

Then enter the code:

NFWM-MWTB
The only AWS account available to you is: 419456231856
Using the account ID 419456231856
The only role available to you is: OaExt-SciTec
Using the role name "OaExt-SciTec"
CLI default client Region [None]: us-gov-west-1
CLI default output format [None]: json
CLI profile name [OaExt-SciTec-419456231856]: titan

To use this profile, specify the profile name using --profile, as shown:

aws s3 ls --profile titan

echo "export AWS_DEFAULT_PROFILE=titan" >> ~/.zshrc
```