# renovate-composer-security-only

We only want to apply security updates but disable everything else for now.

The following should happen
- require-dev:
  - `ergebnis/composer-normalize:^2.20` (`^2.23.1` is available, but should not be updated)
- require:
  - `symfony/console:^5.2` (`^5.4.3` is available, but should not be updated)
  - `composer/composer:^2.1.7` (`^2.2.3` is availble and should be updated because of this [GHSA-frqg-7g38-6gcf](https://github.com/composer/composer/security/advisories/GHSA-frqg-7g38-6gcf))
  
Running renovate on `bitbucket-server` on self-hosted does nothing anymore.
