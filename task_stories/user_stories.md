## User Stories & Object Model Tables

#### Land

```
As an air traffic controller 
So I can get passengers to a destination 
I want to instruct a plane to land at an airport
```

Object | Messages
------------------------------- | ---------------------------------------
controller | 
passenger | 
plane | 
airport | land_plane


#### Take-off

```
As an air traffic controller 
So I can get passengers on the way to their destination 
I want to instruct a plane to take off from an airport
and confirm that it is no longer in the airport
```

Object | Messages
------------------------------- | ---------------------------------------
controller | 
passenger | 
plane | 
airport | take_off

#### Prevent landing when airport is full

```
As an air traffic controller 
To ensure safety 
I want to prevent landing when the airport is full 
```

Object | Messages
------------------------------- | ---------------------------------------
controller | 
passenger | 
plane | 
airport | land_plane
airport | take_off
airport | prevent_landing
airport | full?

#### Airport capacity

```
As the system designer
So that the software can be used for many different airports
I would like a default airport capacity that can be overridden as appropriate
```

Object | Messages
------------------------------- | ---------------------------------------
controller | 
passenger | 
plane | 
airport | land_plane
airport | take_off
airport | prevent_landing
airport | full?
airport | set_capacity

#### Prevent take-off due to weather

```
As an air traffic controller 
To ensure safety 
I want to prevent take-off when weather is stormy 
```

Object | Messages
------------------------------- | ---------------------------------------
controller | 
passenger | 
plane | 
airport | take_off
airport | prevent_take_off
airport | stormy?

#### Prevent landing due to weather

```
As an air traffic controller 
To ensure safety 
I want to prevent landing when weather is stormy 
```

Object | Messages
------------------------------- | ---------------------------------------
controller | 
passenger | 
plane | 
airport | landing
airport | prevent_landing
airport | stormy?

