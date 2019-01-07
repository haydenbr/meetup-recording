# Trouble Shooting

Something at some point will go wrong, but most issues can be resolved!

## General Troubleshooting

It might go without saying, but in all seriousness, turning it off and turning it back / unplugging and plugging it back in will solve most of your problems, whatever "it" is. HDMI cables, Ethernet cables, powered components, projector, microphone, your computer, etc.

## HDMI Problems

One of the most common things to go wrong is HDMI display, whether that's the HDMI signal your feeding to your computer for recording or the HDMI display your pushing back out to the projector from your HDMI over Ethernet emitter.

Depending on what's gone wrong, whether the projector image or your recording signal, you should be able to isolate where the problem might be coming from.

### Projector Image

If the projector is having problems, but your HDMI signal is fine, then there's most likely a problem in the front of the room.

If the projector image is flickering or cutting in and out intermittently, try checking all your HDMI cables. Something as simple as a pinched HDMI cable may cause this. If you have chairs anywhere near your HDMI cables, make sure that none of the chair legs are directly on top of your cables.

If the projector image and HDMI image are both blurry or significantly low quality, and the presenter is using an HDMI to whatever flavor-of-the-month port adapter, it could be a problem with the adapter. I've seen it a few times where the projection was only displaying at 420p, and as soon as we swapped adapters, the projector image jumped to 1080p.

As a last ditch effort, the presenter might have to decrease the refresh rate or resolution their computer is sending over their display port. Ideally, you would be able to find a work around, but this can be an acceptable work-around if nothing else seems to work.

And following the most effective help desk advice, try unplugging and replugging all your HDMI cables. Try turning your HDMI extender off and back on again. Turn the project off and on.

### HDMI Recording Signal

Probably the most common problem with your HDMI recording signal is Ethernet. If you see the HDMI capture flickering in OBS, there's probably an issue with your cable, and it's most likely a bad termination on either end. For this reason, it's a good idea to have backup cables, or keep your Ethernet termination tools handy in case you need to re-terminate on the fly. Once you've made a good termination, the cable should work indefinitely. I've had a few cases, though, where issues didn't manifest until the day of an event, even though I had tested the cable beforehand.

The next thing to check is the [EDID settings](https://en.wikipedia.org/wiki/Extended_Display_Identification_Data) on your HDMI over Ethernet receiver. Your HDMI over Ethernet kit should have come with a user manual. DON'T THROW THIS AWAY. It should tell you how to configure your EDID settings based on your HDMI input. You could have reception issues if these are not properly set.

And as with everything else, off and on / unplug and plug might just solve your problem.

I've never seen this happen, but another possibility is your Ethernet cable is receiving too much electromagnetic interference. This can happen if your Ethernet cables are parallel to electrical cables or in generally "noisy" environments. There's little you can do about this in the moment except for trying to adjust the position of your cables. Shielded Ethernet cable is made to prevent this problem. This will probably never be a problem when recording meetups, but the possibility is always there.

## Recording Problems

At times, you may notice that the video input sources in OBS are a bit jumpy and/or laggy. If this is the case, check the CPU usage in the bottom right-hand corner of OBS. If that percentage gets too high (exactly how high will differ per machine) it can cause recording problems. Also check the bottom left-hand corner of the OBS window. You may see a warning that reads something along the lines of "Encoder overloaded". When one (or both) of these things happen, you'll need to turn down your encoder settings. You can't do this in the middle of recording, so you'll need to be strategic in how you handle this during an event. The specific settings you're looking for are in Settings > Output in OBS, under the Recording tab of Advanced mode or in Settings > Video. You definitely want your video sampling set to 30 FPS, but you might also need to play with bitrate and encoding settings as well.

With all of this said, however, the OBS profile included with this repo is set up in such a way to avoid these kinds of problems.
