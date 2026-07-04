# AWS80ProjectsChallenge

My 80 hands-on AWS projects documentation across compute, networking, security, serverless, IaC, CI/CD, DevOps, data, ML & DR - building toward a Cloud/DevOps role.

Each project lives in its own repository and is linked here as a git submodule, so this repo acts as a central index and portfolio for the full challenge.

## Getting the code

Since the projects are included as submodules, clone with:

```bash
git clone --recurse-submodules https://github.com/simeonprimordial/AWS80ProjectsChallenge.git
```

If you already cloned without that flag:

```bash
git submodule update --init --recursive
```

## Projects

| # | Project | Description |
|---|---------|-------------|
| 1 | [aws-static-website-cloudfront](https://github.com/simeonprimordial/aws-static-website-cloudfront) | Hosting a static website with S3 and distributing it via CloudFront |
| 2 | [aws-wordpress-lightsail](https://github.com/simeonprimordial/aws-wordpress-lightsail) | Deploying a WordPress site on Amazon Lightsail |
| 3 | [aws-ec2-apache-webserver](https://github.com/simeonprimordial/aws-ec2-apache-webserver) | Deploying and configuring an Apache web server on an EC2 instance |


*More projects will be added here as the challenge progresses, covering networking, security, serverless, IaC, CI/CD, DevOps, data, ML, and disaster recovery.*

## Progress

- [x] Project 1 —> Static Website with CloudFront
- [x] Project 2 —> WordPress on Lightsail
- [x] Project 3 —> EC2 + Apache Web Server
- [ ] Projects 4 – 80 —> in progress

## About this challenge

This repository tracks my journey through 80 AWS projects, each documented in its own repo with setup steps, architecture notes, and lessons learned. The goal is to build practical, hands-on experience across the AWS ecosystem as I work toward a Cloud/DevOps role.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
