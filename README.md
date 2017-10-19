# s3staticwebpage
Recipe for hosting a static web page on AWS S3

1. Route 53 purchase domain name e.g. 'colouringin.cc'
2. Wait 24 hours
3. Create S3 bucket (colouringin.cc) and grant public read access to bucket
4. Bucket properties > Static website hosting > Use this bucket to host a website > index.html
5. Make note of endpoint 's3-website-us-east-1.amazonaws.com'
6. Upload index.html and grant public read access
7. Route53 > Hosted zones > colouringin.cc > Create Record Set
8. Alias > Yes > Alias Target: 's3-website-us-east-1.amazonaws.com'
9. Check http://colouringin.cc and confirm index.html displays
