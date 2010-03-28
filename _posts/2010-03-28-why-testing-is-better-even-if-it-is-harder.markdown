---
layout: post
title: Why testing is better, even if it is harder.
categories: eden
---

It's easier not to...
--

I was going to write a blog article stating that I'd never write untested code again. The thing is, that'd probably be a lie. I don't seem to be able to accept, (even in the face of overwhelming evidence to the contrary) that testing is the only way to roll.

Don't get me wrong.
-

Don't get me wrong, I totally get that testing is the right thing to do. I also believe that, but when I am under pressure and have a very short time to get something done, I fall back into bad habits.

I recently had to fix something, it seemed simple. I didn't test it. Far more hours later than it should have been, it's working. It's still not tested, as I don't know how I'd test it. (Anyone with suggestions as to how to test nginx init.d and config files?) 

I spent a long time thinking it was my microscopic sinatra app. It wasn't. It was unrelated, but because I had no tests, I wasn't sure and so kept going around in circles trying to fix a phantom bug.

It was in fact nginx and my init.d script that wasn't actually restarting it, so the changes I made to config.ru or my app made no difference...

The point is, if I'd thoroughly tested my app, microscopic though it was, I'd have known the problem wasn't there.

To quote Yoda (And I know Enrique would!)
--

I was going to say I'd try and always test my code. 

"Do, or do not, there is no try."
