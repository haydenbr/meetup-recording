# Equipment Setup

## Overview

The schematic below provides an overview for a typical setup and how all the components play together. 

<div style="width: 500px;">
	<img alt="equipment-diagram" src="./images/equipment-setup-schematic.png" />
</div>

## Equipment List

Here's a list of all the equipment needed

- (1) USB webcam
- (1) tripod
- (1) USB over Ethernet
- (1) HDMI over Ethernet
- (1) HDMI to USB 3.0 capture card
- (1) USB audio interface
- (1) powered USB 3.0 hub
- (2) 75ft Ethernet cables
- (1) short, 6in - 3ft, HDMI cable
- (1) medium, 3ft - 6ft, HDMI cable
- (1) long, 30ft, HDMI cable
- gaffers tape
- XLR cable(s) as needed
- extension cord(s) as needed
- power strip(s) as needed

## Details

Keep in mind that the above diagram does not take physical distance into account so actual placement of each component might vary widely depending on the venue. Your setup might change based on venue so look at this document as a starting point.

Take note of the devices that need to be powered. You'll want to have enough extension cables handy in the case that a power outlet is not easily accessible from the location at which you need to place one of your powered components (i.e. the USB over Ethernet emitter).

The main concerns in choosing where to setup your equipment are

1) not getting in the presenter's way
2) not blocking the attendees' view and
3) getting the best A/V quality possible.

### Computer Setup

This setup was designed for recording to take place in the back of the venue in order to reduce distraction. This also makes the setup more scalable.

Ideally, you'll want to have your recording computer setup on a table or space in the back of the room. You'll need enough horizontal space for the computer, HDMI over Ethernet receiver, USB over Ethernet receiver, audio interface, USB hub, HDMI capture card, and all the cables involved with these devices.

You'll want to have your computer plugged in while recording. OBS can consume a lot of power while recording, and you'll most likely run out of battery if not plugged in. You need three USB inputs, and the input for the HDMI capture card *must* be USB 3.0. The USB hub is not always necessary, but you will need one if you don't have enough inputs. If using a USB hub, it needs to be powered and needs to be USB 3.0. Otherwise, your input quality will be reduced and that hub will be the weakest link in your setup. If you're using a newer Mac or PC that provides multiple USB-C ports, you're ok using dongles to convert to USB-C. Try to use more than one USB-C port if possible.

### Camera Setup

Set up the camera and tripod in a location that gets a good view of the presenter, but does not block attendees' view. If there's an aisle in your venue, that might be a good option. When possible, try not to get too much of the projector screen in the presenter's background.

Another factor that might impact where you place the webcam is access to a power supply. The USB over Ethernet emitter is a powered device. Technically the emitter does support Power over Ethernet (PoE), but I've seen cases where that does not always work. You can use PoE if it works for you, but just make sure to test it well beforehand.

### HDMI Capture Setup

The main challenge of the HDMI capture portion is setting up the HDMI over Ethernet emitter and the related cables out of the way of the speaker. This can be challenging because there's four cables involved: HDMI cable from the presenters laptop, HDMI cable from emitter's HDMI out port to the projector's input, the Ethernet cable, and the cord for the emitter's power supply. How you handle this really depends on the venue's existing A/V setup.

With a little creativity, there's always a solution. Nicer or more permanent venues might have a ceiling mounted projector and wired podium. In this case, if you can get into the podium's cabinet that houses all of the cables, it should be pretty trivial just to put the emitter in between the existing HDMI cable, and put your own HDMI cable from the emitter's out port into the input that feeds the projector. These podium's usually have additional power outlets inside as well so power for the emitter shouldn't be a problem. This is the ideal case; Everything is hidden inside the podium. If you're not able to get inside the cabinet, you can still make it work, it just might not be as pretty. Main concern though is still to keep everything out of the way the presenter's way.

In other venues, there might just be a single HDMI cable that goes directly to the projector or to a plate in the wall. In this case, it's very likely that the HDMI cable provided by the venue will not be long enough to allow you to set up the emitter out of the way of the presenter. For this reason, it's a good idea to have your own, longer HDMI cables on hand, hence the long HDMI cable in the equipment list. A longer cable will you give you a little more flexibility in where you set everything up.

### Audio Setup

Your audio setup will vary more than anything else, depending on both the venue as well as your equipment. The schematic above has the audio interface plugging directly into your recording computer, which is ideal. If you have a corded mic in the front of the room, it's preferable to connect XLR cable from the mic to your audio interface in the back of the room.

Depending on your set up though, if you need to, you can plug the audio interface into the HDMI over Ethernet emitter (most emitters have multiple ports). It shouldn't make any difference to OBS. Audio quality may be a concern though due to bandwidth and more hops between the audio source and your computer. Placing the audio interface away from your recording computer also makes it more difficult to adjust audio input levels in the middle of an event.

#### Small venues

Smaller venues that don't require audio amplification for the presenter are usually pretty easy. In this case, a microphone is just for the sake of recording. Set up your mic. Plug it into the interface. Connect the interface to your computer, and you're done.

#### Large venues

Large venues with a pre-existing audio setup tend to me more difficult. In these spaces, you usually can't forego audio amplification of your speaker because if the size of the room and number of attendees. This forces you to work alongside the audio system already in place.

You might be able to get an audio output signal from the existing system, which actually makes your life easier. In this case, you don't even need to use your own microphones. Just plug the audio signal into your audio interface. This usually looks like plugging into an XLR output on a sound board somewhere. If you get lucky, the venue will have a box (or boxes) in the floor towards the back of the room somewhere that provide XLR audio output. When you're able to get an audio signal from the venue's system, your effectively using the same sounds system for both recording as well as audio amplification. This is the ideal case for a large venue.

Sometimes though, you won't get so lucky. Some venues may have their audio equipment locked away somewhere, only accessible to a select few internal to the hosting organization. In this worst case scenario, you'll have to settle with dual audio setups: the venue's audio system and your own audio equipment for recording. This *may* be an annoyance to the presenter, depending on how invasive your audio equipment is, as they will have to speak into two mics.

#### Question and Answer

Question and answer sessions are a valuable part of any session. There's two ways you can ensure you properly record this interaction. The first and easiest option is to have your presenter simply repeat any question before giving the answer so as to include the context of the answer for those watching the recording later on. Alternatively, you can provide an additional mic to record any input from the question-asker, assuming your audio interface can handle multiple inputs. This does require extra equipment, extra space, a little more setup time, and time for your attendees to come up to the mic.

#### Other audio concerns

It might go without saying, but do make sure to do a sound check before the start of an event and if possible, before each session if there are multiple sessions, preferably with the actual presenter. 

Audio quality might suffer due to ambient noise coming from A/C units, refrigerators, outside noice, etc. Do as much as you can to reduce this extra noise during events.

When possible, always prefer XLR cables over 1/4" audio cables. XLR provides much greater distance, and they're balanced to protect from external noise. External noise is much more likely to affect 1/4" cables, which are designed for short distances and don't have built-in protection.

## Additional Considerations

### Cables

After everything is set up, do take care to tape down all of your cables with gaffer tape. It might also be helpful to have some cable ties on hand to manage any unruly cables or keep things extra clean.

Make sure to lay out cables out of the way of chairs and as out of the way of people as possible. During an event, keep an eye out for pinched Ethernet or HDMI cables. Pinched cables can cause flickering or temporarily cut off output signals.

Depending on your venue, you may need work outside of the ideal setup to make everything work. Get creative! Keep in mind that XLR and Ethernet cables can cover long distances and there exist ways to extend, adapt, combine, and convert different cables and inputs from one to the other.

Backup cables are a good idea.
