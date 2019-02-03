Your rules go here.
All rule files have to have the ".rules" file extension and must follow a special syntax.

Check out the openHAB documentation for more details:
https://www.openhab.org/docs/configuration/rules-dsl.html

{channel="mqtt:topic:mqtt25er:phcstatus:chan00", autoupdate="false"}
{channel="mqtt:topic:mqtt25er:phcstatus:chan01", autoupdate="false"}
{channel="mqtt:topic:mqtt25er:phcstatus:chan02", autoupdate="false"}
{channel="mqtt:topic:mqtt25er:phcstatus:chan03", autoupdate="false"}
{channel="mqtt:topic:mqtt25er:phcstatus:chan04", autoupdate="false"}
{channel="mqtt:topic:mqtt25er:phcstatus:chan05", autoupdate="false"}
{channel="mqtt:topic:mqtt25er:phcstatus:chan06", autoupdate="false"}
{channel="mqtt:topic:mqtt25er:phcstatus:chan07", autoupdate="false"}

Thing topic phcstatus "phcstatus_thing" {
    Channels:
        Type switch : chan00  [ stateTopic="phcstatus/amd/5/0" , commandTopic="phc/amd/5/0", ON=1, OFF=0 ]
        Type switch : chan01  [ stateTopic="phcstatus/amd/5/1" , commandTopic="phc/amd/5/1", ON=1, OFF=0 ]
        Type switch : chan02  [ stateTopic="phcstatus/amd/5/2" , commandTopic="phc/amd/5/2", ON=1, OFF=0 ]
        Type switch : chan03  [ stateTopic="phcstatus/amd/5/3" , commandTopic="phc/amd/5/3", ON=1, OFF=0 ]
        Type switch : chan04  [ stateTopic="phcstatus/amd/5/4" , commandTopic="phc/amd/5/4", ON=1, OFF=0 ]
        Type switch : chan05  [ stateTopic="phcstatus/amd/5/5" , commandTopic="phc/amd/5/5", ON=1, OFF=0 ]
        Type switch : chan06  [ stateTopic="phcstatus/amd/5/6" , commandTopic="phc/amd/5/6", ON=1, OFF=0 ]
        Type switch : chan07  [ stateTopic="phcstatus/amd/5/7" , commandTopic="phc/amd/5/7", ON=1, OFF=0 ]
    }