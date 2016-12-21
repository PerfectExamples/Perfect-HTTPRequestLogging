# Perfect HTTP Request Logging Example

<p align="center">
    <a href="http://perfect.org/get-involved.html" target="_blank">
        <img src="http://perfect.org/assets/github/perfect_github_2_0_0.jpg" alt="Get Involed with Perfect!" width="854" />
    </a>
</p>

<p align="center">
    <a href="https://github.com/PerfectlySoft/Perfect" target="_blank">
        <img src="http://www.perfect.org/github/Perfect_GH_button_1_Star.jpg" alt="Star Perfect On Github" />
    </a>  
    <a href="http://stackoverflow.com/questions/tagged/perfect" target="_blank">
        <img src="http://www.perfect.org/github/perfect_gh_button_2_SO.jpg" alt="Stack Overflow" />
    </a>  
    <a href="https://twitter.com/perfectlysoft" target="_blank">
        <img src="http://www.perfect.org/github/Perfect_GH_button_3_twit.jpg" alt="Follow Perfect on Twitter" />
    </a>  
    <a href="http://perfect.ly" target="_blank">
        <img src="http://www.perfect.org/github/Perfect_GH_button_4_slack.jpg" alt="Join the Perfect Slack" />
    </a>
</p>

<p align="center">
    <a href="https://developer.apple.com/swift/" target="_blank">
        <img src="https://img.shields.io/badge/Swift-3.0-orange.svg?style=flat" alt="Swift 3.0">
    </a>
    <a href="https://developer.apple.com/swift/" target="_blank">
        <img src="https://img.shields.io/badge/Platforms-OS%20X%20%7C%20Linux%20-lightgray.svg?style=flat" alt="Platforms OS X | Linux">
    </a>
    <a href="http://perfect.org/licensing.html" target="_blank">
        <img src="https://img.shields.io/badge/License-Apache-lightgrey.svg?style=flat" alt="License Apache">
    </a>
    <a href="http://twitter.com/PerfectlySoft" target="_blank">
        <img src="https://img.shields.io/badge/Twitter-@PerfectlySoft-blue.svg?style=flat" alt="PerfectlySoft Twitter">
    </a>
    <a href="http://perfect.ly" target="_blank">
        <img src="http://perfect.ly/badge.svg" alt="Slack Status">
    </a>
</p>

Perfect HTTP Request Logging Demonstration

This project is a simple demonstration of running an HTTP server with HTTP Request logging.

[See the documentation for more detailed description of the Perfect Logging functionality.](https://www.perfect.org/docs/HTTPRequestLogging.html)

## Compatibility with Swift

The master branch of this project currently compiles with **Xcode 8.1** or the **Swift 3.0.1** toolchain on Ubuntu.

## Building & Running

The following will clone and build an empty starter project and launch the server on port 8181.

```
git clone https://github.com/PerfectExamples/Perfect-HTTPRequestLogging.git
cd Perfect-HTTPRequestLogging
swift build
.build/debug/Perfect-HTTPRequestLogging
```

You should see the following output:

```
[INFO] Starting HTTP server  on 0.0.0.0:8181
```

When visiting [http://localhost:8181](http://localhost:8181) in a browser you will see lines like the following flowing into the console:

```
[INFO] [/NzcfGnz8-1] 2016-12-21 13:57:58 GMT-05:00 "GET / HTTP/1.1" from 127.0.0.1 - 200 67B in 0ms
[INFO] [/NzcfGnz8-2] 2016-12-21 13:58:05 GMT-05:00 "GET /hello?world= HTTP/1.1" from 127.0.0.1 - 200 67B in 0ms
[INFO] [/NzcfGnz8-3] 2016-12-21 13:58:18 GMT-05:00 "GET /hello?world=somethings HTTP/1.1" from 127.0.0.1 - 200 67B in 0ms
```

To view the generated log file on disk, open (or tail) the `customHTTPLogFile.log`.

### Xcode

To run the project in Xcode, navigate to the directory in terminal and execute:

```
swift generate xcode-proj
```

Then open the generated project, select the executable scheme, edit the scheme and change the current working directory to the project's directory (so you can see the generated log file more easily). Then Run the project.

## Issues

We are transitioning to using JIRA for all bugs and support related issues, therefore the GitHub issues has been disabled.

If you find a mistake, bug, or any other helpful suggestion you'd like to make on the docs please head over to [http://jira.perfect.org:8080/servicedesk/customer/portal/1](http://jira.perfect.org:8080/servicedesk/customer/portal/1) and raise it.

A comprehensive list of open issues can be found at [http://jira.perfect.org:8080/projects/ISS/issues](http://jira.perfect.org:8080/projects/ISS/issues)



## Further Information
For more information on the Perfect project, please visit [perfect.org](http://perfect.org).
