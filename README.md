# notes-app
Middleman app for rendering provided notes

## Usage
This app uses [middleman](https://middlemanapp.com/) to render notes that you supply. Notes should be located in `source/posts/` and formatted in markdown.

The easiest way to setup this application to render notes is to create a symbolic link from the notes to `source/posts/`, e.g. on OSX/Linux:
```sh
ln -s /path/to/notes/directory ./source/posts
```

Render the notes with:
```sh
bundle exec middleman
```

Dependencies are managed with [bundler](http://bundler.io/) - install it as follows:
```sh
gem install bundler
```

And install the gems by running the following from the cloned-directory

```sh
bundle install
```

## Development

The Ci system used is [concourse](http://concourse.ci). The symbolic-link approach above works well for viewing the notes, but is incompatible with running `fly` locally.

## License and Copyright
Copyright © 2015-2016, Robert Dimsdale. Licensed under [MIT License](https://github.com/robdimsdale/notes-app/raw/master/LICENSE).
