# 300 - Visual Summary

Here's an architecture diagram of the very simple setup we use for Harness CI:

![image](https://user-images.githubusercontent.com/1499433/178939913-9e24f817-f345-49cc-bffb-0b11e40f937e.png)

You will install the Harness Delegate in the same cluster you use for the build farm. The Delegate will create the namespace ```harness-delegate```. You'll use that namespace for both the Delegate and build farm. You can change it if you like.
