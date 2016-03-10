# orchard

Build OSX machine images from scratch.

Directly inspired by [https://github.com/pivotal-sprout/sprout-orchard].


## Prerequisites

1. Use [CreateUserPkg](https://github.com/MagerValp/CreateUserPkg) to make a user, assign a password, and give them an icon.  Upload that package to S3.
1. Upload the latest OSX installer to S3.
1. Upload the latest XCode command line tools to S3.

TODO: Describe setting up Travis or CircleCI.


## Deployment

1. Pick a Mac Mini
1. Make a periodic job to: sync the latest installer, user package, and command line tools
1. Make a periodic job to run orchard and output to the proper path for netboot images
1. Move the orchard artifacts into a DeployStudio target (not automated?)


## Contributing

1. Fork it ( https://github.com/minifast/conference-opportunities/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
