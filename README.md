# ForzaDashboard
Forza Motorsport 7 data-out receiver

What it's intended for:
I'm usually driving manual (sometimes with clutch) and frequent car changes make it difficult to get those upshifts right. I can either focus on the track or on the rpm-display.
The shift-indicators some cars provide also don't help much due to them working differently for each car (growing, flashing, blinking...aaargh!)
Also, a far-off goal is to include data history and further telemetry so that the dashboard helps empirically optimize driving (and tuning) through data analysis per car.

What it does:
This simple dashboard shows a singular shift-indicator all the time, no matter which car I'm driving in and how many rpm the engine can do.

the shift indicator is customizable by car to limit the range for low-revving cars and increase it for high-revving cars so as not to miss your perfect shift.

the shift indicator is based on measured max. rpm. Not the (data-out) max rpm which is the display-limit. The measured rpm are stored per car and by default, the shift indicator maximum is set to 99% of those max measured rpm - that way you don't hit the limiter.

It also shows other information such as current rpm, speed (kph/mph), calculated acceleration and deceleration, and many of the other data-out values.

You can name your car (If anyone of you can produce a list of car ordinals (data-out) with corresponding names, I'll gladly import them)

If you figure out a way to loopback the data-out stream, you can also use the "always on top" feature, using the dashboard as an overlay, positioning it over your ingame dashboard (in windowed mode)

Listening Port configurable in .properties file - standard port is 1337.

Maximizing, Resizing, dragging without the windows bar on top cluttering the info-display.

(some) car data stored in .properties file - for each car that you've actually driven using the dashboard. so after a while, It could be complete.


What it is not:
The dashboard is just a first draft.
There are sure to be bugs in it (like the ugly drag-resizing or the hiccups with car names of cars not yet in the config file).
I intend to include all data-out datapoints in an readable fashion (think telemetry display like the overlay in FM itself) at some point.