---
layout: post
title:      "Handling multiple STDIN inputs"
date:       2020-08-12 18:21:34 +0000
permalink:  handling_multiple_stdin_inputs
---


I recently completed a HackerRank challenge that required me to handle multiple inputs using the method gets. Gets is the Ruby method equivalent of reading STDIN for those following who are familiar with other languages. I needed a container to hold all the STDIN coming in so I could then alter them. Pushing them into an array seemed like a solid idea, which I immediately thought of, except when I added the code to push, it only accepted one input.

I tried to get more information on STDIN itself and how it works and there wasn’t much information on my specific issue. I decided to do a bit of playing around with the output of gets. In my example I needed to handle 3 input values and I was only receiving one. I then attempted to output gets 3 times. I successfully receive the 3 values that were input. How did I get them?

To my understanding, STDIN only holds 1 string of value at a time. Calling gets each time allowed the other inputs to then replace the preceding ones. My very first value was an integer (that was a string I needed to convert to an integer). I saved this initial value to a variable that I would later use for a condition in the following loop. This loop, with a condition to end based on a built-in counter incrementation, would then push the gets into my input array.

Here’s the example code:

Note - My first STDIN was an integer, 2


```
input = []
counter = 0
a = gets.to_i

until counter == a
    counter += 1
input << gets
end
```


The rest of the challenge was easy to deal with, but I have never experienced handling input previously. I hope this helps whoever is reading this.

Once again, Happy Coding!!!

