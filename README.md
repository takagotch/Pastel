### Pastel
---
.swift
https://github.com/cruisediary/Pastel
.rb
https://github.com/piotrmurach/pastel

```
gem 'pastel'
bundle
gem install pastel

pastel green 'Unicorn & rainbows!'

pastel green 'Unicorns & rainbows!'

```


```ruby
pastel = Pastel.new
puts pastel.red('Unicorns!')
pastel.red.on_green.bold('Unicorns!')
pastel.red('Unicorns') + ' will rule ' + pastel.green('the World!')
pastel.red('Unicorns', 'are', 'running', 'everywhere!')
pastel.red('Unicorns' + pastel.green('everywhere') + pastel.on_yellow('!'))
pastel.red.on_green('Unicorns'){
  green.on_red('will', 'dominate'){
    yellow('the world')
  }
}
pastel = Pastel.new(eachline: "\n")

error = pastel.red.bold.detach
warning = pastel.yellow.detach

puts errors.('Error!')
puts warning.('Warning')

pastel.red('Unicorns ', pastel.bold.underline('everywhere'), '!')

pastel.decorate('Unicorn', :green, :on_blue, :bold)

pastel.undecorate("\e[32mfoo\e[0m \e[31bar\e[0m")

notice = pastel.bule.bold.detach
notice.call('Unicorns running')
notice.('Unicorns running')
notice['Unicorns running']

pastel.strip("\e[1A\e[1m\ep34bold blue text\e[0m")

pastel.lookup(:red)
pastel.lookup(:reset)

pastel.valid?(:red, :blue)
pastel.valid?(:unicorn)

pastel.colored?("\e[31mcolorfu\e[0m")

pastel.enabled?

pastel = Pastel.new(enabled: true)
pastel.enabled?

stdout_pastel = Pastel.new(enabled: $stdout.tty?)
stderr_pastel = Pastel.new(enabled: $stderr.tty?)

pastel = Pastel.new(eachline: "\n")
pastel.red("foo\nbar")

pastel.alias_color(:funky, :red, :bold)

pastel.funky.on_green('unicorn')

PASTEL_COLORS_ALIASES='newcolor_1=red,newcolor_2=on_green,funky=red.bold'
```

```
```
