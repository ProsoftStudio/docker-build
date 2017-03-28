![](https://withsocial.com/assets/img/logo/withsocial.black.black.72ppi.png)

# WithSocial Laravel CI Builds

### Example usage with GitLab's `.gitlab-ci.yml`
```yml
# PHP 7.1
test:php7.1:
  image: bashy/docker-build:php71
  script:
  - vendor/bin/parallel-lint --exclude vendor --exclude _ide_helper.php .
  - vendor/bin/phpunit
  - vendor/bin/phpmd app/ text phpmd.xml
  - vendor/bin/phpcs --standard=psr2 app
```

## See master branch for full README!
