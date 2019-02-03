Your thing definitions go here.
All thing files have to have the ".things" file extension and must follow a special syntax.

Check out the openHAB documentation for more details:
https://www.openhab.org/docs/configuration/things.html

Thing topic phcamd03 "phcamd03_thing" {
    Channels:
        Type switch : chan00  [ stateTopic="phcstatus/amd/3/0" , commandTopic="phc/amd/3/0", ON=1, OFF=0 ]
        Type switch : chan01  [ stateTopic="phcstatus/amd/3/1" , commandTopic="phc/amd/3/1", ON=1, OFF=0 ]
        Type switch : chan02  [ stateTopic="phcstatus/amd/3/2" , commandTopic="phc/amd/3/2", ON=1, OFF=0 ]
        Type switch : chan03  [ stateTopic="phcstatus/amd/3/3" , commandTopic="phc/amd/3/3", ON=1, OFF=0 ]
        Type switch : chan04  [ stateTopic="phcstatus/amd/3/4" , commandTopic="phc/amd/3/4", ON=1, OFF=0 ]
        Type switch : chan05  [ stateTopic="phcstatus/amd/3/5" , commandTopic="phc/amd/3/5", ON=1, OFF=0 ]
        Type switch : chan06  [ stateTopic="phcstatus/amd/3/6" , commandTopic="phc/amd/3/6", ON=1, OFF=0 ]
        Type switch : chan07  [ stateTopic="phcstatus/amd/3/7" , commandTopic="phc/amd/3/7", ON=1, OFF=0 ]
    }

    {channel="mqtt:topic:mqtt25er:phcamd02:chan00"}
    {channel="mqtt:topic:mqtt25er:phcamd02:chan01"}
    {channel="mqtt:topic:mqtt25er:phcamd02:chan02"}
    {channel="mqtt:topic:mqtt25er:phcamd02:chan03"}
    {channel="mqtt:topic:mqtt25er:phcamd02:chan04"}
    {channel="mqtt:topic:mqtt25er:phcamd02:chan05"}
    {channel="mqtt:topic:mqtt25er:phcamd02:chan06"}
    {channel="mqtt:topic:mqtt25er:phcamd02:chan07"}