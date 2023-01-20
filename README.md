# Welcome to the "cs" repo.

"cs" is a simple tool for making it easy to create C# Solution repo's containing multiple C# Projects, 
from the command line.

------

I'm a C# newbie.  Creating a C# repo is more complicated than I expected... complete with magical XML files 
that somehow get managed by Visual Studio, which, I am told, I don't have to worry about.  

I worry when people say stuff like that.

What if I just want to use VS Code?  Or even develop something from the command line?  Both things seem quite 
reasonable to me, given the multi-language, multi-OS, multi-cloud multiverse we live in.

This repo is my attempt to learn by doing, creating a tool for making it easy to create repos (C# "Solutions")
which contain multiple loosely coupled collections of code (C# "Projects").  When I add a new C# Project to
my repo, I get some boilerplate code, complete with unit test, that invites me to flesh out the code (and the
test) in a TDD way.

## Installation

All we need to do is pull down "cs" into our local git directory;  and we can start using it to build
other repos.  If you put your git repo's in ~/gits, then this might go like this:
 
```bash
cd ~/gits
git clone git@github.com:danholle/cs.git
```

I can now verify my .NET environment, as well as installation of "cs", as follows:
```bash
cd cs
dotnet test
```

You should get back an indication that 3 tests passed, and none failed.

## Usage

Now you want to save the world. using C#.  Let's roll!

First, we create the repo, under your name, on git.  Git isn't really comfortable with C# yet, even 
though it's owned by Microsoft.  Life is like that sometimes.

On your fave browser, go to
```
https://github.com/yourname
```

and click the big green New button on the top right.  Create your repo named "SaveTheWorld" which 
is something of a C#esque repo name.  Git will ask if you want a .gitignore file.  Nice offer,
but he doesn't know how to do it for C#, so decline the generous offer.

Now, where were we?  Ah, yes, the command line.
```bash
cd ~/gits
git clone git@github.com:yourname/SaveTheWorld.git
cd SaveTheWorld
../cs/initrepo
```
The last command, unsurprisingly, initialises your new repo, adding a C# .gitignore and setting
up the C# solution environment (SaveTheWorld.sln).


NEED TO ADD THE ADDER EXAMPLE AND SHOW TESTING FRAMEWORK

------

## Good Night

It is after midnight, so if I go to bed now, I'll have successfully gone to bed "early".

More later.

May the Force be with you.




```bash
cd 
