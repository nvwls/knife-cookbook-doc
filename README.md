knife-cookbook-doc
==================

This is a Knife plugin to generate a skeleton `README.md` file from a cookbook's
`metadata.rb` file.

The plugin helps to

- create the first bits of documentation you can build upon
- write documentation that is consistent among your or your team's cookbooks
- implement the [DRY/SPOT](http://c2.com/cgi/wiki?DontRepeatYourself) rule
  (`metadata.rb` is the authoritative source of information)


Installation
------------

You can install the plugin via RubyGems:

    $ gem install knife-cookbook-doc

Alternatively, you can install the plugin from source:

    $ git clone git://github.com/realityforge/knife-cookbook-doc.git
    $ cd knife-cookbook-doc/
    $ bundle install
    $ bundle exec rake install

Afterwards, the new knife command `knife cookbook doc DIR` will be available.


Usage
-----

    knife cookbook doc COOKBOOK_DIR (options)

        -o, --output-file FILE           Set the output file to render to relative to cookbook dir. Defaults to README.md
        -t, --template FILE              Set template file used to render README.md

    Examples:

        knife cookbook readme from path/to/cookbook
        knife cookbook readme from path/to/cookbook --template README.md.erb


License
-------

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.


Contact
-------

* Web: <http://mlafeldt.github.com/knife-cookbook-readme>
* Mail: <mathias.lafeldt@gmail.com>
* Twitter: [@mlafeldt](https://twitter.com/mlafeldt)
