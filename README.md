# Oystercard Challenge

A project that creates an oystercard to travel in London

The aim of this challenge is to - 
- I write code that is easy to change
  - Writing easy to change software is highly prized amongst developers and employers. By developers because most of a developer's time is spent changing software. By employers because their teams can deliver value to customers faster.
- I can test-drive my code
  - Tested software is easier to change because you can tell when it's broken just by running a command, even the tricky edge cases.
- I can build with objects
  - Most code in the world is structured in small pieces called objects. This is done because it is easier to change than having everything in one place.
  
### How to use 
- Clone this repo to your machine
- Run bundle install
- Run from the terminal
```
require './lib/Oystercard'
card = Oystercard.new
=> card @balance=0, @max_bal=90, @entry_station=nil

card.top_up(10)
=>10
card.touch_in("Kings Cross")
=> "Kings Cross"
card
=> card @balance=10, @max_bal=90, @entry_station="Kings Cross"
card.in_journey?
=> true
card.touch_out
=> nil
card
=> card @balance=9, @max_bal=90, @entry_station=nil
card.in_journey?
=> false
```

### User Stories 
```
In order to use public transport
As a customer
I want money on my card
```
```
In order to keep using public transport
As a customer
I want to add money to my card
```
```
In order to protect my money
As a customer
I don't want to put too much money on my card
```
```
In order to pay for my journey
As a customer
I need my fare deducted from my card
```
```
In order to get through the barriers
As a customer
I need to touch in and out
```
```
In order to pay for my journey
As a customer
I need to have the minimum amount for a single journey
```
```
In order to pay for my journey
As a customer
I need to pay for my journey when it's complete
```
```
In order to pay for my journey
As a customer
I need to know where I've travelled from
```
```
In order to know where I have been
As a customer
I want to see to all my previous trips
```
```
In order to know how far I have travelled
As a customer
I want to know what zone a station is in
```
```
In order to be charged correctly
As a customer
I need a penalty charge deducted if I fail to touch in or out
```
```
In order to be charged the correct amount
As a customer
I need to have the correct fare calculated
```
### Status
- I managed to get up to and complete the user story that asks for the customer to be able to know where they have travelled from. 
- All tests are passing
