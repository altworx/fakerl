     _______    ___       __  ___  _______ .______       __
    |   ____|  /   \     |  |/  / |   ____||   _  \     |  |
    |  |__    /  ^  \    |  '  /  |  |__   |  |_)  |    |  |
    |   __|  /  /_\  \   |    <   |   __|  |      /     |  |
    |  |    /  _____  \  |  .  \  |  |____ |  |\  \----.|  `----.
    |__|   /__/     \__\ |__|\__\ |_______|| _| `._____||_______|


*Fakerl* is an Erlang application that generates fake data for you.
Whether you need to bootstrap your database, create good-looking XML documents,
fill-in your persistence to stress test it, or anonymize data taken from a production service, Faker is for you.

Fakerl is a port of Python's [Faker][python-faker], and was motivated
by a need for a bunch of fake data for writing test suites.


*work in progress*


## How it works

At the core of fakerl is a simple template parser that maps template variables to module functions.

```erlang
My name is {{name}}.
My email address is {{email_address}}, and I am currently located in {{address}}
```

Each time the template above is parsed, a random name, email address, and location address
will be generated. This fake data is generated by data generators written in Erlang.

## Generators

The following fake data generators are available:

* Names
* Person
* Datetime
* Addresses
* Profile
* Company
* Lorem
* Internet

## Documentation

```erlang
make docs
```

## Tests

```erlang
make tests
```

## TODO

see the bundled TODO file

## License

Fakerl is released under the MIT Licence. See the bundled LICENSE file for details.


Contributing
-------------
Issues, forks, and pull requests are welcome!


Credits
--------

- [joke2k][joke2k] / [Faker][python-faker]


[python-faker]: https://github.com/joke2k/Faker "Python faker"
[joke2k]: https://github.com/joke2k "joke2k"
