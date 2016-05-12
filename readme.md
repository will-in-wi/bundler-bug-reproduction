# Test for Bundler limits

```
% vagrant up
% vagrant ssh
$ cd /vagrant
$ bundle install
```

Observed output:

```
vagrant@precise64:/vagrant$ bundle install
Fetching gem metadata from https://rubygems.org/
Fetching version metadata from https://rubygems.org/Retrying fetcher due to error (2/4): ThreadError can't create Thread: Resource temporarily unavailable
Retrying fetcher due to error (3/4): ThreadError can't create Thread: Resource temporarily unavailable
Retrying fetcher due to error (4/4): ThreadError can't create Thread: Resource temporarily unavailable
[HANGS]
```