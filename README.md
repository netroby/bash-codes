## List file in directory and empty them
find . -type f -exec sh -c 'cat /dev/null > "{}";' \;
## Tar the git diff --name-only
tar zczf new-files.tar.gz `git diff --name-only 4cbe7..HEAD`
## Delete remote git branches which already been deleted
git remote prune $(git remote)

## Donate me please

![Scan QRCode donate me via Alipay](https://www.netroby.com/assets/images/alipayme.jpg)

**Scan QRCode donate me via Alipay**
