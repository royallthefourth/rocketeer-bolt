# rocketeer-bolt
Example Rocketeer deployment configuration for Bolt CMS

To setup an existing Bolt site to use Rocketeer, first make a copy of your site somewhere.
1. Import your code into git. Use the example .gitignore to avoid committing user uploads and vendor libraries. Rocketeer will manage the uploads in their own directory and install libraries.
1. Place the .rocketeer directory in your project root. Edit the files to suit your configuration.
1. Run `rocketeer deploy` to send your code out to the server.
1. Copy the contents of your `web/files` directory from the copy of your old site to the new `shared` directory like so:
    `cp -R ../example.com.old/web/files/* shared/web/files/`