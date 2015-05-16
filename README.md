# Zrspec

Determine to use zeus to run rspec if it's running.

## Installation

Add this line to your application's Gemfile:

    gem 'zrspec'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install zrspec

## Usage

Run by `zrspec`

    $ zrspec

If zeus is running, it's equal to

    $ zeus rspec

Or it will be equal to

    $ rspec

## Integration

To run rspec with zeus in [sublime-text-2-ruby-tests](https://github.com/maltize/sublime-text-2-ruby-tests), you may set up the configuration like this
```
{
  "run_rspec_command": "zeus rspec {relative_path}",
  "run_single_rspec_command": "zeus rspec {relative_path}:{line_number}"
}
```
But this will has problem without running zeus. In this time, you can install this gem and set up to
```
{
  "run_rspec_command": "zrspec {relative_path}",
  "run_single_rspec_command": "zrspec {relative_path}:{line_number}"
}
```
It will work both cases.

## License
The project is released under the [MIT license](http://www.opensource.org/licenses/MIT).

## Contact
The project's website is located at https://github.com/emn178/zrspec  
Author: emn178@gmail.com
