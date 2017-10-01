# RageMP Gitlab Continuous Integration Config

How to run : 

1. Install gitlab runner from https://docs.gitlab.com/runner/ on your server and configure it with your repo
2 Add gitlab-runner to sudoers and make it passwordless :

```sudo usermod -a -G sudo gitlab-runner && sudo sh -c "echo \"gitlab-runner ALL=(ALL) NOPASSWD: ALL\" >> /etc/sudoers"```
3. Add .gitlab-ci.yml to your gitlab repository

The create.sh file will generate and register a systemd service.
