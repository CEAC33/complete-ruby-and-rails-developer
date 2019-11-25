# complete-ruby-and-rails-developer

## Intro & Setup

https://repl.it/languages/ruby

```ruby
address = [1, 2, 3, 4, 5, 6, 7, 8, 9]
p address
p address[5]
new_address = address.reverse!
p new_address
```

### Ruby on Rails Development Environment overview

**Development Environments**
- To develop web applications you will need to create a development environment
- To develop web applications using Ruby on Rails, you will need Ruby (the language) and Ruby on Rails (the web app framework) installed

**Options**
- Cloud based IDE's, Ruby on Rails: Amazon Web Services Cloud9, Regular Cloud9 (only available through educator accounts), Codeanywhere etc., I use nitrous in a lot of the videos but nitrous isn't available anymore, but it's similar to a lot of other ones so it's very easy to follow
- Local IDE's - Rubymine by Jetbrains
- Simple local Development environment (free at best for long term): Combination of Terminal window/Command prompt, (powershell) and a code editor

AWS Cloud9:
- https://aws.amazon.com/es/cloud9/

RubyMine:
- http://www.jetbrains.com/ruby/

Atom:
- https://atom.io/

Sublime Text:
- https://www.sublimetext.com/3

### Mac - Setup Local Development Environment

**Install Ruby on Rails on a Mac**

- Ensure either x-code or x-code command line tools are installed and updated
  - Thi may be the reason for some errors you face
- Ensure Homebrew is installed and working correctly - may be errors in this step. Don't overlook them. Update brew
- Get a ruby version manager to move around multiple versions of Ruby effortlessly
  - I use RVM and it's a choice of many
- Install Ruby using rvm
- Update gem (RubyGems - a Ruby package manager)
- Use gem to install bundler and nokogiri (this might take a bit of time)
- Use gem to install Rails
- Get a text editor to write code in - I use atom, lots of people use sublime

**X-Code or X-Code Command line Tools**

- http://railsapps.github.io/installrubyonrails-mac.html
- http://railsapps.github.io/xcode-command-line-tools.html > Is Xcode Already Installed?

```bash
$ xcode-select -p
/Applications/Xcode.app/Contents/Developer
```

**Homebrew**
- https://brew.sh/

```bash
$ brew doctor
```

```bash
$ brew update
```

**RVM & Ruby**
- http://rvm.io/rvm/install
- http://railsapps.github.io/installrubyonrails-mac.html > Install RVM

```bash
$ \curl -L https://get.rvm.io | bash -s stable
```

Close and Reopen your Terminal

- http://railsapps.github.io/installrubyonrails-mac.html > Install Ruby
- http://rvm.io/rubies/default

```bash
$ rvm install ruby-2.5.1
```

```bash
$ rvm list
```

```bash
$ rvm use 2.5.1
```

```bash
$ ruby -v
```

```bash
$ rvm list
```

**Update Gem, install Bundler & Nokogiri**

- http://railsapps.github.io/installrubyonrails-mac.html > Check the Gem Manager

```bash
$ gem -v
```

```bash
$ gem update --system
```

```bash
$ gem install bundler
```

```bash
$ gem install nokogiri
```

```bash
$ gem install rails -v 5.1.6
```

```bash
$ rails -v
```

```bash
$ ruby -v
```

**Get a Text Editor**

Atom:
- https://atom.io/

Sublime Text:
- https://www.sublimetext.com/3

## The Ruby Programming Language

### How to get Free Live Help

- https://discordapp.com/invite/0fcPkObEsGTjNSvQ

### Intro to Ruby

- http://www.ruby-lang.org/en/

**Running it on Repl**
- https://repl.it/languages/ruby

```ruby
# Say hello world in multiple ways
# Simple put string
# Using a variable
# Using a method

print "Hello World\n" # it doesn't include the newline
puts "Hello World" # returns Nil
p "Hello World" # return the string

greeting = "Hello World"

puts greeting

def say_hello(thing_to_say)
  puts thing_to_say
end

say_hello "Hello World Ruby is grat!"
```

**Running it locally**

```bash
$ touch playground.rb
```

<blockquote> <code><b>playground.rb</b></code> <pre>
p "Hello World" # return the string
</pre> </blockquote>

```bash
$ ruby playground.rb
```
