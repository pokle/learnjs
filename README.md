# LearnJS

A Serverless Single Page App demo / scratch pad from the book.

https://pragprog.com/book/brapps/serverless-single-page-apps

Running at http://learn.shonky.info/

## Infrastructure

Static site is hosted on AWS:

    Route53 CNAME learnjs.shonky.info 
      => CloudFront distribution with HTTPS Cert d1as0ohsaesuhb.cloudfront.net 
        => S3 Static hosting learnjs.shonky.info.s3-website-ap-southeast-2.amazonaws.com 
          => S3 bucket learnjs.shonky.info 


## Develop

  npm install -g livereloadx
  ./sspa liveserver

## Deploy

  ./sspa deploy_bucket learnjs.shonky.info

## Change Log

### Beta 3 Changes

  * Compensating for AWSCLI timing issues when creating roles
  
### Beta 2 Changes

  * Now using 'admin' profile instead of default profile
  * Added create_service action to sspa
  * deploy_bucket can now take a config path

## MIT License

Note: The license below applies only to the contents of this git repository, not the Pragmatic Bookshelf title "Serverless Single Page Apps", or any other related content.

Copyright (c) 2015 Ben Rady <benrady@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Creative Commons Attributions

  * HeroImage.jpg is licensed from popularwoodworking.com under the Creative Commons Attribution License (CC BY 3.0 US).
