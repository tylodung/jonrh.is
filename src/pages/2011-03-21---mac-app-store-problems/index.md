---
title: Mac App Store problems
date: "2011-03-21T00:00:00Z"
path: "/mac-app-store-problems/"
---

<!-- Todo: Adapt links to Markdown -->

If you're here because the <a href="http://www.apple.com/mac/app-store/">Mac App Store</a> is
giving you troubles then you've come to the right place. In my search I found
<a href="http://discussions.apple.com/thread.jspa?threadID=2728270&amp;tstart=60">two</a>
<a href="http://discussions.info.apple.com/message.jspa?messageID=12890660">distinct</a> problems
and solutions.

If you're having troubles signing in (the login window doesn't appear or you can't type anything in
the input boxes) then it might be because you're running
<a href="http://unsanity.com/haxies/fruitmenu">FruitMenu</a> or
<a href="http://unsanity.com/haxies/ape">Application Enhancer</a>. Apple has acknowledged that
problem here <a href="http://support.apple.com/kb/TS3638">http://support.apple.com/kb/TS3638</a>.
If you don't want to disable FruitMenu then
<a href="http://www.cnet.com/profile/fcarroll/">fcarroll</a> suggests a workaround:
<blockquote>There is a relatively easy workaround for this problem. When an attempt is made to log
in to the App store with Fruit Menus running, the log in window appears behind the main window
instead of in front. If the main window is moved out of the way, the log in window will be visible.
You can't type into it but, using the contextual menu, the password can be pasted and the log in
button can be clicked.</blockquote>

If you get a never ending loading screen that reads "One moment please. Connecting to the Mac App
Store. Loading..." then you'll need to delete two files and restart.

![The One moment please loading screen for the Mac App Store](./mac_app_store_one_moment_please.png)

To delete the files paste the two lines below into
<a href="http://answers.yahoo.com/question/index?qid=20081006182950AAX1h6m">Terminal</a> and press
enter:

```
rm ~/Library/Preferences/com.apple.appstore.plist
rm ~/Library/Preferences/com.apple.storeagent.plist
```

I did stumble upon another
<a href="http://pbagwl.com/post/2873882667/mac-app-store-fix-one-moment-please">very similar
solution</a> by Paul Bagwell but it deletes some extra folder. If deletion of the two files plus a
restart didn't help I'd definitely give that solution a try. If you find some other
problems/solutions please post in the comments and I'll update the post.

<!--

Comments:

2012.09.12 AT 20:31, Roger:
Thanks jonrh, perfect. I was on the phone with Apple tech and he had no clue what my problem was.
Went to terminal, deleted the two files from terminal and wala!! Thanks for the info and help. Now
I can download FCP X and Mountain Lion finally!!

-->