+++
title = '12th Spring 2024 Meeting'
date = 2024-04-11T12:13:25-04:00
draft = false
summary = 'next semester meeting times, general discussion'
tags = ['meeting', 'tech news', 'elections', 'schedule']
+++
***
# Overview
- Attendance
- Meeting
***
## Attendance
- Abu Shettima
- Christian Messmer
- Lavender Wilson
- Matthew Williams
- Paul Shriner
- Jonathan Buckel
- Joshua Watson
## Meeting
We did not have anything in particular planned for this meeting, so it was mostly focused on smaller discussions.

### Rust Vulnerability
There was a recent command line injection vulnerability found in Rust. It affects programs on Windows that use Rust's `std::process::Command` to both run a batch file _and_ allow the user to add arguments to the `Command`. 

Here is an example of a piece of code that would be affected:  
```Rust
use std::io::{self, Write};
use std::process::Command;

fn main() {
	println!("enter payload here");
	let mut input = String::new();
	io::stdout().flush().expect("Failed to flush stdout");
	io::stdin().read_line(&mut input)
			   .expect("Failed to read from stdin");

	let output = Command::new("./test.bat") // <- requirement 1
						  .arg(input.trim()) // <- requirement 2
						  .output()
						  .expect("Failed to execute command");\
	println!("Output:\n{}", String::from_utf8_lossy(&output.stdout));
}
```  
This exact scenario must be met in order for this vulnerability to be exploited (only on Windows). In this piece of code, any malicious user can input any system command to be executed on the host system. 

This is a lesson in input: you should _always_ sanitize input from your user.

### Next Semester Meeting Times
Since most of our core members were here for the meeting, we wanted to figure out what times/days would be good now that common hour is gone.

We decided that it would currently be best to meet on __Tuesdays__ from __5-6__, both in-person (most likely the same as usual, __Eberly 342__), as well as including online users who can't make it there in person. This decision, however, is not set in stone and may change. 

### Other Topics
There were many other smaller discussion topics, including:
- Linux
- Officer Nominations
- Common hour
	- :(
- Summer Projects
	- Find something to work on over the summer
	- Try to meet with other people in the club to track progress/keep motivation up
- Waveform collapse algorithms
