# Sinatra Helpers

## javascript

simply call `javascript 'path/to/js', 'path/to/another', ...` to queue
javascript files you would like to use, then call `javascript` (without
any args) to output the include tags (or embed the all the javascript if
in production)

## css

same deal as `javascript`, call `css 'path/to/css', ...` then call `css`
again without any args to output the link tags (doesn't support embedding
the concatenated files for production like `javascript` does. (not yet
anyways.)

## Disclaimer

These helpers can be used in any project and are not limited to Sinatra (e.g. could be easily used in Rails.) That being said, they are by no means a completed product and were simply hacked together for a Sinatra project.

### TODO

* Embed a single include tag for `javascript` in production rather than raw javascript.

* Concatenate css into single link tag for `css` in production

* Write tests and refactor

* Compile into gem for use in any Rack project

* Add native support for Rails

