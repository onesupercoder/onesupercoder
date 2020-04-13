---
title: "Install Graalvm EE  with SDKMAN and Set It Up for Inttellij"
date: 2020-04-12T14:03:06-06:00
---

To download GraalVM EE Navigate to: https://www.oracle.com/technetwork/graalvm/downloads/index.html

![Oracle GraalVM EE Downloads Page](/images/install-graalvm-ee-and-set-it-up-for-inttellij/graalvm-downloads.png)

Select the Java Version and the Operating System.  You'll have to create a free Oracle Account if you don't have one already here: https://profile.oracle.com/myprofile/account/create-account.jspx

Once downloaded you'll need to extract to a location.  If you're using SDKMAN then I would recommend you extract it to a location in ~/.sdkman/candidates/java/[VERSION]  replace with your downloaded version.  Mine is 20.0.0.r11.ee. R11 being the jave version or use R8, R14 for Java 8 and Java 14.

{{< highlight shell >}}
$ tar -xzvf graalvm-ee-java11-darwin-amd64-20.0.0.tar.gz
$ mv graalvm-ee-java11-20.0.0 ~/.sdkman/candidates/java/20.0.0.r11.ee
{{< / highlight >}}

Then whn you open IntelliJ navigate to: File -> Project Structure -> Platform Settings -> SDKs.
If you click the + button it should automatically detect the JDKs like it did for me:

![Intellij Project Structure JDKs](/images/install-graalvm-ee-and-set-it-up-for-inttellij/intellij-jdks.png)


Inspired by: https://e.printstacktrace.blog/installing-graalvm-ee-1-0-0-rc14-with-sdkman/