# code_generator (base)

Base (and first) template for generate cookbooks. It's based on chef-dk 0.9.0 code_generator. See *details* section to have more informations about it.

## Usage

1. Reference the code_generator cookbook directory (this directory) when using `chef` to generate a new cookbook

### Example

```
chef generate cookbook my_cookbook -g SOMEPATH/chef-generators/base/code_generator
```

### Defaults

The following Chef generators variables were overrided to fill the Mindera requirements:
* Name of the copyright holder - 'Mindera'
* Email address of the author - 'social@mindera.com'
* Licence - 'MIT'


## Details

At this moment this repo only provides a Cookbook generator. Based on https://github.com/chef/chef-dk/tree/master/lib/chef-dk/skeletons/code_generator it also creates Gemfile with a gem dependency to cookbook_sdk found in https://github.com/Mindera/cookbook_sdk/tree/master
