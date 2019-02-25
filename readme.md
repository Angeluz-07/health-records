# Computerization of Health Records
Minimal implementation of computerization of health records in Erlang.

## Requirements
- Install Erlang on Ubuntu 18 `sudo apt-get install erlang`

## Usage
### Setting environment
1. Open a terminal and place in project's directory
2. Compile with `make`
3. Start erlang shell `erl`

### Functions
- `bmi:compute({Weight,Height}).`
- `heartRate:max(Age).`
- `heartRate:target(Age).`
-  `HP1 = #healthProfile{firstName="Bob",lastName="Lee",age=23,height=1.7,weight=75}.`

### Examples

```
>> bmi:compute({75,1.7}).
{overweight,25.95155709342561}

>> heartRate:max(20).
200

>> heartRate:target(20).
{100.0,160.0}

>>rr("healthRecord.hrl").
>>#healthProfile{age=23,height=1.7,weight=75}.
#healthProfile{firstName = undefined,lastName = undefined, age = 23,height = 1.7,weight = 75}
```
