# Pummeldoge

An example Rails app that uses the [LayerVault API](https://developers.layervault.com).

What does it do? It makes sweet GIFs and MOVs of your work, like so:

![](https://f.cloud.github.com/assets/47004/1696657/1fb2ed20-5ec8-11e3-9487-5a2c28d1b427.gif)

## Installation

pummeldoge is a Rails 4 application. You will need [gifsicle](http://www.lcdf.org/gifsicle/), 
[ffmpeg](https://trac.ffmpeg.org/wiki/MacOSXCompilationGuide), 
and [imagemagick](http://stackoverflow.com/questions/7053996/how-do-i-install-imagemagick-with-homebrew) installed.

You will also need to register a LayerVault application. You can do that from your [LayerVault Development](https://layervault.com/settings/development) page. 
(Account required. Accounts are free.)

Next, define your API keys in your shell:

```
export LAYERVAULT_CLIENT_ID=MY_LAYERVAULT_CLIENT_ID_FROM_THE_SITE
export LAYERVAULT_CLIENT_SECRET=MY_LAYERVAULT_SECRET_FROM_THE_SITE
```

Then:

```
git clone git@github.com:layervault/pummeldoge.git
cd pummeldoge
bundle
bundle exec rails s
open http://localhost:3000
```

Hot doge!