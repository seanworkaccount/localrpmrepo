How to make a local rpm git lfs repository
fist, make a directory on your system, then set it up so it's tracked by git
after that download git lfs and set up your repository to track rpm files using the dollowing command while cd'd into your repository
  git lfs track "*.rpm"
now whenever you push a commit including rpm files those rpm files will be tracked by lfs
more information about git lfs can be found here: https://docs.github.com/en/repositories/working-with-files/managing-large-files/configuring-git-large-file-storage

Now to make sure that your repository is recognized as a repository you need to use create repo to generate the metadata for your repo and write a repository config file for your repo
this process is described in depth step by step here: https://www.percona.com/blog/how-to-create-your-own-repositories-for-packages/
