# Internet issues

All the data (except the mobile screenshot) is captured by the script included

The tl;dr of the script is that it hits google with an http request, times it and records the result then schedules another call in 100ms

The script was run on my laptop while tethered to my phone

The code times out after 130s which is why you dont get numbers any bigger

The two graphs represent the time taken for said http request

The ```date```  field is when the request _started_, ```took``` is in seconds

Over time

![Over time](https://raw.githubusercontent.com/jamesstow/internet_issues/master/error_dashboard_screenshop.png)

An hour or so long segment

![Hour segment](https://raw.githubusercontent.com/jamesstow/internet_issues/master/one_hour_dashboard_screenshot.png)

Ookla speedtest on phone (obviously only consider the ones for ```2020-08-05```

![Ookla](https://raw.githubusercontent.com/jamesstow/internet_issues/master/phone_speedtests.jpg)

You can see some form of repeating pattern in the errored requests (just over two minute intervals)

Any missing periods are when I stopped the script running

The request data was put into a database and I configured a grafana instance to look at it to view the data (grafana dashboard also included)
