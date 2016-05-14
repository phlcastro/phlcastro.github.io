---
layout: post
title:  "How to handle random values on RSpec unit tests"
date:   2016-05-13 23:02:00 +0000
categories: ruby rspec tdd
---
When I was coding this [exercise][beinglucky] in Ruby, I decided to use `Random.rand` to simulate a roll of dices.
Obviously this led me with a problem of how to code unit tests on RSpec and set the expected result using random values?

Actually, the solution is pretty simple (as you can see bellow): all you need to do is a method stub. A method stub is an implementation that returns a pre-determined value.

<script src="https://gist.github.com/phlcastro/41edf06a5439c906dc5460a01afd744e.js"></script>

For more details, [you can check RSpec docs here][rspec].

[beinglucky]: https://github.com/phlcastro/beinglucky
[rspec]: http://www.relishapp.com/rspec/rspec-mocks/v/3-4/docs/configuring-responses/returning-a-value