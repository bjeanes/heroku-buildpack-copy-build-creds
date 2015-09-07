# Runtime creds buildpack

This copies your compile-time `~/.ssh`, `~/.netrc`, and `~/.curlrc` files to the app directory.

This files are usually created with other buildpacks such as https://github.com/bjeanes/ssh-private-key-buildpack or https://github.com/timshadel/heroku-buildpack-github-netrc

## Should I use this?

Probably not. These creds belong at compile time for a reason. This exists for the few limited cases where your app needs run-time access to things like GitHub. This buildpack exists to be composed with other buildpacks (such as those mentioned above) to avoid duplicating their functionality here.

## License

MIT
