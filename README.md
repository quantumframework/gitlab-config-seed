# GitLab Configuration as Code

## Assumptions

- GitLab webhooks are transmitted over an internal network with
  an internal CA; the default value of ``hook_validate_certs``
  is therefore ``false``.

## Caveats

- Due to a bug in the ``gitlab_hook`` module, use of tokens
  on webhooks is not supported. We therefore recommend to use
  this project only on a secured internal network.
