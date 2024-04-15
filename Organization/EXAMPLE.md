# Organization Example
Our example is going to first show the layout of the Organization and then it will show what **I think** is the best organization structure I've seen.

As a point of fact, the layout of the organization is representative of a heirarchical tree as seen below.
![Organization](https://github.com/Phoneyboi/dataModelTeamcenter/assets/90519425/317d26a0-5377-4bfa-8167-5d81320b8d2b)

With this structure in mind, I will show you what **I think** is the best organizational structure I have seen below. This is specifically a Group for Engineering. When you look at this example, think to yourself "**If I want to release Engineering data, what roles do I need to define in my organization**"?

![Organization Example](https://github.com/Phoneyboi/dataModelTeamcenter/assets/90519425/775c2a57-d4c8-42cc-bf6a-26e7a515228c)

Obviously, this should be modified to your business needs but it solves our initial Should and Should Not criteria. This organizational structure is simple, it defines a role called Senior Engineer that can review and release data in Teamcenter, and it defines a role Mechanical Engineer that is not allowed to review and release data in Teamcenter; likewise for Electrical Engineering. There is an added Drafter role which is meant to be a role that only authors data, not particularly for approval of data. 

This is not an all encompassing layout, but provides a good foundation to the Teamcenter Organization. One way to extend this is to ask yourself what other types of engineering data need to be released; Manufacturing, Materials, etc. These can be added as Sub-Groups to the Engineering Group. 
