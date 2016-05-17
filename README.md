# AlfredGit
Helps you handle multiple git repos more quickly and easily.

## Longer Description
Guys. We live in 2016. Cars are out there driving *themselves*. We are *half a
century* removed from sending a man to another celestial body and without even
blowing him up in the process. Why on Earth (heh), then, do I need to cd into
every single repo I'm working with on a project and type individual git commands
in every one of them?

You know, some guy back in the 20s had a similar question. Why did he have to
do all this stupid 'math' crap by hand? And do you know what he did? He punched
math in the face and invented freaking computers (I don't know my computer
history very well). I...well, to be honest, I'm doing something a tad less
monumental, but I am that man. A modern what's-his-name-you-know-the-guy-who-
hated-math-and-invented-computers-if-that-story-is-even-real(-it's-not).

Enter AlfredGit, named after a certain famous billionaire's butler. AlfredGit does
those stupid menial typing tasks for you. Why? Because you're freaking Batman
and Batman doesn't have time to sit there cd-ing into 12 different repo
directories and issuing a `git pull` in every single one of them. He's too
busy out there punching...uh...bugs and...feature requests. In the face (this
analogy is quickly falling apart). So grab AlfredGit and say goodbye to
spending 20% of your day typing git commands in 140 different repos like a
pleb. This, guys. This is the future.

# Installation

I'd recommend holding off on this for right now, as I'm planning on gem-ifying
this soon enough. Once that's done, an install will be as easy as typing `gem
install alfred` or something similar. Pretty sure someone already took that
gem name even though their app doesn't even compare and doesn't deserve the
moniker.

# Use

I've tried to make the command syntax as intuitive as possible. Essentially,
you'll send in a few parameters (the exact number of parameters required
changes based on what git command you need to run - you can't run a `git
checkout` without a branch name, for instance) separated by spaces; the repos
you want to work with *always* come last and will also be separated by spaces.

AlfredGit comes packaged with the most common git commands built in, but also
allows you to send custom commands! If your first parameter doesn't match
any of the built-in commands, the first parameter itself will be the command
that is run! Simple! Think another command warrants being on this list?
Email me and I'll consider adding it!

And with that, we come to the built-in commands. Here are the AlfredGit commands
followed by a description of what they run. Most of these should be intuitive.

* `pull` - Runs a `git pull`
* `push` - Runs a `git push`
* `checkout second_parameter` - runs a `git checkout second_parameter`
* `commit second_parameter` - Runs a `git commit -m second_parameter`
* `status` - Runs a `git status`
* `branch` or `branches` - Lists the branches your repos currently have
                           checked out.

# Quick Example
Here's a quick example of how it works!

Want to pull repos 1, 2, and 3? Easy!

`> alfred_git pull repo_1 repo_2 repo_3`

What about pulling everything?

`> alfred_git pull all`

How about checking out a branch on multiple repos at once?

`> alfred_git checkout branch_name repo_1 repo_2`

See? Intuitive! Simple! Batman!

## License
The MIT License (MIT)

Copyright (c) 2016 Chris Sellek

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.