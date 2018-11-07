Pint templates
==============

### `sles12sp2.templ`

Sample template for creating a SLES12 SP2 instance based on the latest version
as advertised by SUSE Public Cloud Information service. This template only
works in AWS regions that support Lambda. Please note that creating a stack
based on this template requires the capability `AWS::IAM::Role`. When using the
aws cli, add parameter `--capabilities CAPABILITY_IAM` to the `create-stack`
command line.

### `sles15.templ`

Same for SLES 15.


### Custom template

The templates can be easily modified to create other OS instances. Simply
change the `OS` parameter in the `AMIInfo` block to match the first part
of the image name (before the version string) as reported by `pint` (see
https://www.suse.com/c/riddle-me-this/ for information about `pint`)
