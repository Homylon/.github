# Homylon

**A home automation language you can read.** Plain-text scenes say how a house should behave, and the
Homylon engine makes it happen through small agents for Philips Hue, Zigbee and Z-Wave (MQTT),
Matter, CoAP gateways, sound and more.

```text
define home jensenhouse latitude 52.09 longitude 5.12
when time sunset then light livingroom on warmwhite brightness 40 fade 3
when motion on frontdoorsensor and time between 23:00 and 07:00 then
    light hallway on brightness 10
end
```

**The engine, the agents, the apps, the manual and the Jensens: [homylon.org](https://www.homylon.org)**

## Here on GitHub

The open parts, MIT licence:

| Repository | What |
|---|---|
| [homylon-protocol](https://github.com/Homylon/homylon-protocol) | how programs talk to the engine: PROTOCOL.md |
| [homylon-kit-swift](https://github.com/Homylon/homylon-kit-swift) | the network layer for Swift apps, tools and agents (Apple platforms and Linux) |
| [homylon-monitor](https://github.com/Homylon/homylon-monitor) | the Monitor for iPhone/iPad, Mac and Apple TV: shows live what the engine does, and a complete example of an app |

Homylon runs at home, on a Mac, a Linux box or a Raspberry Pi. Nothing leaves the house unless you
let an agent do it.
