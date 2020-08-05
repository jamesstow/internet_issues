# Internet issues

All the data (except the mobile screenshot) is captured by the script included

The tl;dr of the script is that it hits google with an http request, times it and records the result then schedules another call in 100ms

The code times out after 130s

The two graphs represent the time taken for said http request

Over time

![Over time](https://github.com/jamesstow/internet_issues/error_dashboard_screenshop.png)

An hour or so long segment

![Hour segment](https://github.com/jamesstow/internet_issues/one_hour_dashboard_screenshot.png)

Ookla speedtest on phone (obviously only consider the ones for ```2020-08-05```

![Ookla](https://github.com/jamesstow/internet_issues/phone_speedtests.jpg)

You can see some form of repeating pattern in the errored requests (just over two minute intervals)

Any missing periods are when I stopped the script running

The request data was put into a database and I configured a grafana instance to look at it to view the data (grafana dashboard also included)
