
# INSTALL

```
git clone -b news.academical.io git@github.com:LaxWorks/news.git news && cd $_

git submodule init && git submodule update

mkdir vendor && pushd $_
curl -L -O https://mirror.racket-lang.org/installers/6.7/racket-6.7-x86_64-linux.sh
chmod +x racket-6.7-x86_64-linux.sh
sudo ./racket-6.7-x86_64-linux.sh --unix-style --dest /usr/ --create-dir
rm -f racket-6.7-x86_64-linux.sh
popd

sudo yum install rlwrap -y -q

./run-news
```
