# The ScalaBridge Documentation Project

**TODO** - add a build status when we deploy this

## Overview

This documentation has been adapted from the [RailsBridge documentation](http://docs.railsbridge.org). We thank RailsBridge for paving the way for ScalaBridge!

This is a Sinatra app. The ScalaBridge documentation project is home to a few subprojects, including the ScalaBridge installfest instructions, which leads students through the various complicated setup instructions for getting Scala, Java, Git, etc. installed on their computer (whatever combination of computer, OS, and version they happened to bring to the workshop!), as well as the ScalaBridge workshop curriculum.

Each subproject (a "site") comprises files stored under the "sites" directory; for instance, the installfest instructions are located at ROOT/sites/en/installfest, while the intro scala curriculum can be found under ROOT/sites/en/intro-to-scala. (The "en" means "English" -- see "Locales" below.)

These files can be in any of these formats:

* `.step` for [StepFile](step_file_reference.md)
* `.md` for [Markdown](http://daringfireball.net/projects/markdown/syntax)

(If multiple files exist with the same base name, `.step` is preferred over `.md`
## Usage

    bundle install
    bundle exec rake run

If the above fails (say, because `rerun` doesn't work on your system), try

    rackup

Then open <http://localhost:9292> in a web browser, and verify that you can navigate the installfest slides.

## Locales

We do not yet support different Locales!

## Contributing

TODO - [CONTRIBUTING.md](CONTRIBUTING.md)

Check out [CONTRIBUTING.md](CONTRIBUTING.md) to see how to join our [list of contributors](https://github.com/scalabridge/docs/contributors)!

## License

The documentation (including anything under the `sites` subdir as well as some hardcoded text elsewhere) is licensed under a Creative Commons license ([CC-BY,  specifically](http://creativecommons.org/licenses/by/3.0/)), which means you're welcome to share, remix, or use our content commercially. ScalaBridge has adapted this from RailsBridge, so we ask that any attribution goes to RailsBridge.

## Other Resources

- [StepFile Reference](step_file_reference.md)
- **TODO** - Workshop organizers: See http://docs.scalabridge.org/workshop for example slide decks you can use in your opening/closing presentations.

