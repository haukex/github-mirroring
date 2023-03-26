How to Mirror a GitHub Repository
=================================

This repository contains an example workflow showing how to mirror a GitHub
repository to another remote repository.

1. In the remote repository, configure an access token that has the appropriate
   rights to push to the repository. (For example, on GitLab, the default
   configuration may be that only Maintainers are allowed to push to Protected
   branches.)

2. In your GitHub repository, go to the repository settings and create a new
   secret in "Actions secrets and variables" which holds the token.

3. Take the file `.github/workflows/github-mirror.yml` from this repository and
   adjust the URL so it points at the remote repository and includes the
   authentication information from the secret. **Do not** put any sensitive
   information in this file; put this into the secret instead.

