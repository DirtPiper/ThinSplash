![ThinSplash](/thinsplash.png)

ThinSplash is (to be) a home broadcast software suite consisting of the following programs:

## Schedule Builder

For creating programming blocks, with granularity of minutes, hours, days, weeks, months, seasons, years, etc.

## DVTedit

For ingesting raw video files and imbuing them with the metadata needed to slot them into blocks as commercials or programming

## GuideGen

For automatically generating day-by-day TV guides based on the block programs created in Schedule Builder, as well as distributing footage/guides to ThinCast clients

## ThinCast

For actually airing the final broadcast program based on the guides created by GuideGen

# Design guidelines:

- Implemented in Java (5? 8?)

- DVTedit transcodes all ingested video into h.265 mp4 files at 640x480 @ 60 FPS - maybe allow for HDTV later on

- Hub and spoke topology - one central server hosts the entirety of footage and generates TV guides for a given channel, ThinSplash clients running ThinCast will only need to store at most two days' worth of footage at a time and will download needed footage from the server daily - download tomorrow's lineup, play today's, delete tomorrow's.

# Why?

The authors of ThinSplash experienced, without knowing, the pinnacle of broadcast television. This is our way of keeping it alive, in a way.

# Is ThinSplash legal?

ThinSplash is only the software required to prepare and air video for TV-style broadcast, we do not provide any video footage or other intellectual property.
