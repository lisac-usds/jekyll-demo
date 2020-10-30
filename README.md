# Jekyll Demo

A boilerplate Jekyll website configured to deploy a password-protected site to cloud.gov (Cloud Foundry).


## About the boilerplate Jekyll website

produced by:
```
 $ gem install bundler jekyll
 $ jekyll new jekyll-demo
```

running the site locally:
```
 $ bundle exec jekyll serve
```

See [jekyll](https://jekyllrb.com/).


## cloud.gov

### Configuration
- [manifest.yml](./manifest.yml)
- [Staticfile](./Staticfile) 
- Staticfile.auth (basic authentication, optional)
   > <username-1>:<encrypted-password>
   > <username-2>:<encrypted-password>

### Deployment

> prerequisites: Cloud Foundry cli ([docs](https://docs.cloudfoundry.org/cf-cli/install-go-cli.html)) and [cloud.gov access](https://cloud.gov/docs/getting-started/accounts/)

1. Log in: `cf login --sso`
2. Deply: `cf push`

See: [Staticfile Buildpack](https://docs.cloudfoundry.org/buildpacks/staticfile/index.html)
