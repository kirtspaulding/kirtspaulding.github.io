Wayne Aune 
Uh, welcome to learn that they have these handy to you, especially when he got SQL back end. We're we're not touching it. We're we're going right to you. So it's my lack of experience as well. I thought it was just a file move. 

0:1:1.810 --> 0:1:10.260 
Wayne Aune 
You know, move them up there, go from his on Prem SharePoint so that the plan was 10 to 1313 to 1616 off to SharePoint online. 

0:1:11.350 --> 0:1:20.380 
Wayne Aune 
But we get hung up. We just we, we we get these sync errors and sync errors and 40 hours of waiting and it would start over and you know it it just. 

0:1:21.300 --> 0:1:21.790 
Kirt Spaulding 
OK. 

0:1:21.470 --> 0:1:26.200 
Wayne Aune 
Uh just would, and I know there was some OU issues and there's. 

0:1:27.610 --> 0:1:32.330 
Wayne Aune 
Umm yeah, things that can't speak to because I'm the sales guy, but. 

0:1:31.990 --> 0:1:34.80 
Kirt Spaulding 
OK. Yeah, so. 

0:1:33.280 --> 0:1:41.950 
Wayne Aune 
So try try it, all of it, or Troy will have his arms are on that cause. You again. He was he was digging into the servers and helping out to. 

0:1:44.300 --> 0:1:45.510 
Wayne Aune 
And he should be on soon. 

0:1:47.350 --> 0:2:1.750 
Kirt Spaulding 
OK. Yeah. So you know there there, there's a lot of complexity to what you know what what is trying to be accomplished here, right? But we'll talk about that shortly. Hi, Troy. 

0:2:1.440 --> 0:2:1.770 
Wayne Aune 
All right. 

0:2:2.900 --> 0:2:9.90 
Wayne Aune 
Troy, I just stumbled through what I thought happened, but you're gonna have to. You're gonna have to be more technically. 

0:2:10.380 --> 0:2:10.640 
Troy Heitmann (Guest) 
OK. 

0:2:12.430 --> 0:2:15.160 
Wayne Aune 
And I think that's it. It's just you and Lance, Troy. 

0:2:16.240 --> 0:2:17.170 
Troy Heitmann (Guest) 
I do believe so, yes. 

0:2:17.910 --> 0:2:19.320 
Wayne Aune 
All right. You're really quiet too. 

0:2:20.930 --> 0:2:22.240 
Troy Heitmann (Guest) 
As it is that better? 

0:2:22.960 --> 0:2:23.200 
Jerry Franks 
Yep. 

0:2:25.140 --> 0:2:27.70 
Wayne Aune 
OK, so so let's do introductions. 

0:2:29.450 --> 0:2:33.20 
Wayne Aune 
I've never. I just met Jerry last week. He he is the. 

0:2:33.920 --> 0:2:39.900 
Wayne Aune 
Sales guy for a red level and then he have Kirt, who I just met. Now, who is gonna be the. 

0:2:41.140 --> 0:2:42.400 
Wayne Aune 
Technical leader on this. 

0:2:43.530 --> 0:2:45.990 
Wayne Aune 
Troy is is the. 

0:2:46.770 --> 0:2:53.360 
Wayne Aune 
Worker be that helped us where that was working with Adam our engineer and then lamps as the IT director. 

0:2:56.460 --> 0:2:58.570 
Wayne Aune 
You may can't hear you, but we can see a Lance. 

0:2:59.300 --> 0:2:59.970 
Wayne Aune 
So hello. 

0:3:0.950 --> 0:3:1.980 
Wayne Aune 
So Troy. 

0:3:2.960 --> 0:3:9.160 
Wayne Aune 
Umm. I just told them the path we you're on SharePoint 2010, SQL back end SQL is. 

0:3:9.730 --> 0:3:10.700 
Troy Heitmann (Guest) 
SharePoint 13. 

0:3:11.230 --> 0:3:12.70 
Jerry Franks 
13 yeah. 

0:3:15.260 --> 0:3:17.150 
Wayne Aune 
And SQL back. What's your sequel back in? 

0:3:17.750 --> 0:3:18.470 
Troy Heitmann (Guest) 
UH-14. 

0:3:18.950 --> 0:3:19.320 
Wayne Aune 
Alright. 

0:3:20.930 --> 0:3:23.300 
Wayne Aune 
So we try to help him out. Why don't you take him too? 

0:3:24.30 --> 0:3:27.300 
Wayne Aune 
I I try to hack my way through it, so once you go ahead and tell the story. 

0:3:28.900 --> 0:3:31.930 
Troy Heitmann (Guest) 
OK, so initially our. 

0:3:33.160 --> 0:3:47.600 
Troy Heitmann (Guest) 
Original server SP 2010 had I guess a reporting system or a an attached database to the existing farm for reporting purposes. I I don't know what was all in it. 

0:3:48.930 --> 0:3:49.560 
Troy Heitmann (Guest) 
Although. 

0:3:50.700 --> 0:4:16.840 
Troy Heitmann (Guest) 
Of course, during the migration, um do believe there was some sort of expectation somewhere that it was requesting for for this and the prerequisite was to deploy the service prior to putting the server or migrating the server. So it's it caused a ton of errors that I have documented it in a ticket 11 and total 4 warnings. 

0:4:19.630 --> 0:4:22.210 
Troy Heitmann (Guest) 
But and then I also wanted to check. 

0:4:23.190 --> 0:4:23.940 
Troy Heitmann (Guest) 
With. 

0:4:27.580 --> 0:4:41.650 
Troy Heitmann (Guest) 
With the logs and figuring out which ones are in legacy, off still or which ones had or error messages migrating to the from legacy to. 

0:4:41.900 --> 0:4:43.110 
Troy Heitmann (Guest) 
I I don't. 

0:4:42.730 --> 0:4:43.650 
Kirt Spaulding 
Claims based. 

0:4:44.140 --> 0:4:52.340 
Troy Heitmann (Guest) 
Yeah. Claims based. Thank you. Just to verify that the accounts are no longer in our in our domain or whatever that may be. 

0:4:52.410 --> 0:4:52.670 
Troy Heitmann (Guest) 
Me. 

0:4:54.220 --> 0:5:2.90 
Troy Heitmann (Guest) 
Those, those were pretty much the two big ticket items and according to some Microsoft KB they are not KB, I'm sorry. 

0:5:3.560 --> 0:5:14.390 
Troy Heitmann (Guest) 
Information like about migrating from 10 to 13 um, they said to kind of work them in order and and kind of crush them out. So I I have all the errors. 

0:5:15.790 --> 0:5:16.260 
Troy Heitmann (Guest) 
Recorded. 

0:5:17.670 --> 0:5:18.580 
Troy Heitmann (Guest) 
So just. 

0:5:20.50 --> 0:5:25.450 
Troy Heitmann (Guest) 
I can pass those that information off if you need it, but that's all I got. 

0:5:27.10 --> 0:5:35.960 
Kirt Spaulding 
OK. And did Lance drop, is it is it important that he's here while we're talking about this or is it mainly? 

0:5:37.280 --> 0:5:37.690 
Kirt Spaulding 
We're. 

0:5:38.920 --> 0:5:39.550 
Kirt Spaulding 
OK. 

0:5:37.490 --> 0:5:43.510 
Wayne Aune 
It's, it's Troy like lances, Lance, like, still listening and you just pull that a million different ways. 

0:5:44.360 --> 0:6:13.790 
Kirt Spaulding 
OK, sounds good. Alright. So a couple of questions. Well actually First off, I know that Wayne here introduced me, but my name's Kirt Spaulding. I'm the modern work solution here or solution lead here at red level. So my purview is pretty much every, you know, SharePoint, one drive teams down to the Office Suite, Excel, PowerPoint and the productivity suite as well. So planner, project, et cetera. 

0:6:14.330 --> 0:6:22.920 
Kirt Spaulding 
I got a couple projects that are actually relatively similar to this one, just not as say regulated. 

0:6:24.240 --> 0:6:40.760 
Kirt Spaulding 
But that's me and and nice to nice to meet you as well. So a couple of questions. So you started off in SharePoint 2010 and you were able to at least mostly successfully upgrade to SharePoint 2013, is that correct? 

0:6:41.500 --> 0:6:43.660 
Troy Heitmann (Guest) 
Yes, we are standing at the moment, yeah. 

0:6:44.930 --> 0:6:47.240 
Kirt Spaulding 
OK. Umm and then. 

0:6:48.370 --> 0:6:59.220 
Kirt Spaulding 
The errors in the warnings that you reference those are I guess, still still existing. They resulted from that initial migration or initial upgrade. 

0:7:0.180 --> 0:7:0.650 
Troy Heitmann (Guest) 
Correct. 

0:7:1.700 --> 0:7:3.930 
Kirt Spaulding 
OK. Umm and then. 

0:7:4.600 --> 0:7:16.110 
Kirt Spaulding 
So what? What's the end goal here? And a couple of different questions. You know the the notes that I got was that, you know, BCS is looking to move to SharePoint online. 

0:7:17.290 --> 0:7:46.680 
Kirt Spaulding 
However, you know, can you can you expand a little bit on that? Are we looking at a potentially hybrid scenario? I also need to know about your identity setup, whether it's you know, is it hybrid identity or you running Active Directory domain services and having that coexistence with Azure AD, some of those details. So if you could just expand on like you know the scope of this migration and what the goal is? 

0:7:47.800 --> 0:8:17.670 
Troy Heitmann (Guest) 
The goal is to be 100% cloud. We do we have already performed a Azure AD migration. We're working through some issues right now with with Colin another side and tech, but essentially all of our groups should now be synced. We have a slight problem on that front where some objects were moved into the the deleted users and so there's error messages on deletion, but the main scope for this project is to lift 100% cloud and retain. 

0:8:17.770 --> 0:8:25.840 
Troy Heitmann (Guest) 
The existing structure of our on Prem system like for permissions and stuff so. 

0:8:27.20 --> 0:8:29.50 
Troy Heitmann (Guest) 
And doling out those permissions. 

0:8:33.520 --> 0:8:33.950 
Kirt Spaulding 
Sure. 

0:8:30.810 --> 0:8:35.560 
Troy Heitmann (Guest) 
You know, because it's already in place. We we'd like to. We'd like to retain. 

0:8:34.880 --> 0:8:39.800 
Kirt Spaulding 
Yeah, it made it. Don't need to reinvent the wheel on that security model, right? 

0:8:40.130 --> 0:8:40.370 
Troy Heitmann (Guest) 
Yep. 

0:8:41.860 --> 0:8:49.890 
Kirt Spaulding 
What? What migration tools are you using? Like the SharePoint migration tool, the share gate? What do we got? 

0:8:51.920 --> 0:8:57.740 
Troy Heitmann (Guest) 
I recommended for Adam when he initially started the project for Microsoft Tool. 

0:8:59.260 --> 0:8:59.550 
Lance 
Yeah. 

0:8:59.870 --> 0:9:0.900 
Troy Heitmann (Guest) 
I don't know. 

0:9:2.300 --> 0:9:2.750 
Lance 
You heard. 

0:9:2.20 --> 0:9:6.650 
Troy Heitmann (Guest) 
Off the top of my head, what it's called, but it is a essentially pre. 

0:9:8.480 --> 0:9:10.820 
Troy Heitmann (Guest) 
Pre-check prior to migration from. 

0:9:12.350 --> 0:9:20.100 
Troy Heitmann (Guest) 
Tooth for migrating directly from an on Prem to cloud like a direct migration to to check for pre like. 

0:9:20.950 --> 0:9:21.920 
Troy Heitmann (Guest) 
For future errors. 

0:9:20.750 --> 0:9:52.960 
Kirt Spaulding 
Yeah, I think you're you're might be referring to the the S match SharePoint migration assessment tool. It generates a report that basically brings up all of the potential conflicts. As you probably know, any custom workflows, anything that's connected to business data, so like web parts, if they're surfacing data from those SQL content databases using BDC, business data connectivity, that is not going to migrate, it has to be recreated. 

0:9:53.180 --> 0:10:1.240 
Kirt Spaulding 
Uh, any workflows, whether it's nintex or InfoPath or or things like that won't be migrated with that tool. 

0:10:2.480 --> 0:10:30.630 
Kirt Spaulding 
And so on and so forth. First smaller migrations. You know the Microsoft assessment tool and the Microsoft SharePoint migration tool are generally appropriate. But you know, given the need to kind of maintain the security structure, the groups and things like that, you may be better off using something like share gate, which is gonna be better equipped to, you know, maintain and deal with. 

0:10:31.550 --> 0:10:40.430 
Kirt Spaulding 
Uh, deal with, deal with those things and also it has capabilities that allow you to continually monitor your, your environment and make make changes. 

0:10:41.140 --> 0:10:55.320 
Kirt Spaulding 
Umm, so I think the point of that, I don't know that based on the limited information I have right now, I don't know that the Microsoft free tool is gonna get you where you need to go. 

0:10:59.180 --> 0:10:59.770 
Lance 
Diplomat. 

0:11:1.190 --> 0:11:1.540 
Lance 
Sure. 

0:10:56.800 --> 0:11:5.630 
Troy Heitmann (Guest) 
Yeah, it it wasn't me. That was it was a recommended tool that I provided to Adam. I don't know if it was used, but that's the only resource that I gave. 

0:11:8.140 --> 0:11:34.770 
Kirt Spaulding 
OK. Well, on the uh, I guess you can call it. On the bright side, if if they did or whether they did or did not run the assessment tool, the results of the assessment will help produce and kind of an inventory of of some of the conflicting features and give you an idea of what you know what has to be recreated or what do we need to do to surface the data in SharePoint online. 

0:11:35.410 --> 0:11:37.560 
Kirt Spaulding 
Umm so. 

0:11:38.850 --> 0:11:52.240 
Kirt Spaulding 
What one moment here. Ohh. What's what's your current timeline? You know, and are there any, like, critical deadlines that we're looking at? I know SharePoint Server 2013, I think an April reaches like end of support. 

0:11:53.640 --> 0:11:57.820 
Kirt Spaulding 
You know how? How does the timeline look for VCs internally? 

0:11:58.620 --> 0:11:58.870 
Lance 
Ohh. 

0:12:0.10 --> 0:12:0.870 
Lance 
Would you like to get? 

0:11:59.660 --> 0:12:2.200 
Wayne Aune 
Well, we started this thing about two years ago, but. 

0:12:2.440 --> 0:12:2.790 
Wayne Aune 
Yeah. 

0:12:2.20 --> 0:12:14.610 
Lance 
Yeah, I mean we're we're behind on getting it is there, is there something specific that that our world's gonna end? No, but we're kind of sick of being in the middle of this migration for several months. 

0:12:17.460 --> 0:12:17.970 
Lance 
The work. 

0:12:16.430 --> 0:12:27.90 
Kirt Spaulding 
Oh, sure, if you've got data living in multiple places and you know some some, sometimes I gotta go to the server side. Sometimes I gotta go to SharePoint online. I mean, you know, if the. 

0:12:26.420 --> 0:12:30.720 
Lance 
Well, it's not your point. Online is not functional for us right now. 

0:12:32.350 --> 0:12:32.980 
Kirt Spaulding 
OK. 

0:12:33.370 --> 0:12:56.500 
Lance 
We're not off the ground and and Troy's in the process right now of of, you know, getting that that AD sync, which if I heard right, is we are syncing up now that finally got done. So we just we just want what what what's the what are the tools we need and what's the road map to get us up there? This is not we have to be up there next Tuesday. 

0:12:57.180 --> 0:13:2.230 
Lance 
But you know how? How do we get the tools and and get a process in place? 

0:13:3.110 --> 0:13:5.310 
Lance 
That's going to complete the project. 

0:13:7.560 --> 0:13:8.190 
Lance 
Sense. 

0:13:6.810 --> 0:13:21.360 
Kirt Spaulding 
Right. OK. And something that you just mentioned there, um that the AD Connect sync is set up, so you are running a hybrid identity environment. Does that at least currently and you're looking to? 

0:13:22.660 --> 0:13:25.490 
Kirt Spaulding 
Sunset that and have it be full Azure AD. 

0:13:28.130 --> 0:13:33.820 
Troy Heitmann (Guest) 
Sorry, I guess I misunderstood what you meant. From the SharePoint side, it's gonna be 100% cloud. 

0:13:39.110 --> 0:13:39.460 
Kirt Spaulding 
Right. 

0:13:40.190 --> 0:13:40.640 
Kirt Spaulding 
OK. 

0:13:40.250 --> 0:13:40.840 
Lance 
There you go. 

0:13:35.500 --> 0:13:40.990 
Troy Heitmann (Guest) 
The hybrid model I think is here to stay for the Azure AD, so yes. 

0:13:41.920 --> 0:13:45.520 
Kirt Spaulding 
OK. In terms of like the? 

0:13:46.900 --> 0:14:12.470 
Kirt Spaulding 
Say application strategy you know have have you done like mapping of how you want say SharePoint online to be used and have you considered things like how teams is going to be used or have there been any like say project artifacts or strategy documents. You know do you have a plan basically for the business functionality of the tools? 

0:14:13.580 --> 0:14:14.270 
Lance 
No. 

0:14:15.260 --> 0:14:17.750 
Lance 
Uh, you know, here's. 

0:14:21.490 --> 0:14:22.740 
Lance 
We are. 

0:14:23.850 --> 0:14:25.620 
Lance 
Our our our goal. 

0:14:26.530 --> 0:14:29.360 
Lance 
Is to come up with a migration plan. 

0:14:30.30 --> 0:14:30.570 
Lance 
That. 

0:14:32.400 --> 0:14:44.610 
Lance 
You know, we we don't even have a budget. We don't have the steps for a full, you know, my migration plan for Viking to be, have a larger presence in the cloud. 

0:14:45.720 --> 0:14:49.170 
Lance 
We're still too, Prem, heavy as a company. 

0:14:50.270 --> 0:14:50.740 
Kirt Spaulding 
OK. 

0:14:50.140 --> 0:14:59.380 
Lance 
Umm, So what we've what we've done. You know, we've been we've been buying, you know office product licenses through 365 for a few years. 

0:15:0.750 --> 0:15:19.80 
Lance 
Prior to that, you know it was using volume licensing and buying a license and perpetual license and put it on a machine or buy a machine with a license. And so we we kinda, you know sort of got into the Microsoft Cloud and at least started buying things. 

0:15:19.860 --> 0:15:24.10 
Lance 
By subscription for new users. 

0:15:25.620 --> 0:15:32.710 
Lance 
So we've done that and then you know, of course, you know, Visual Studio for users as a subscription and that kind of crap. 

0:15:33.930 --> 0:15:34.510 
Lance 
Our. 

0:15:35.170 --> 0:16:6.180 
Lance 
Instance of SharePoint was on site. It was 2010 and that was end of life on, you know running on a 2008 server. I do believe and so our impetus, you know this year or last year was OK, let's let's migrate it up to the cloud. Let's get this company a little more cloud oriented, working with Wayne and the guys at Seton. They said look you know for us to really give you support. 

0:16:6.430 --> 0:16:24.940 
Lance 
Let's transfer your products to us as a as a reseller, you know, so they're, you know yet that that super ISO up and up and up above you all. So we've done that with all the subscriptions we can couple we have to wait till they play out. 

0:16:26.180 --> 0:16:31.700 
Lance 
And we engaged with them to move SharePoint up to Azure. 

0:16:33.460 --> 0:16:36.560 
Lance 
That has turned into a bit of a boondoggle. 

0:16:37.690 --> 0:16:48.760 
Lance 
We tried to go right from 210 all the way up to Azure and as it turns out, Microsoft deprecated the products to do that that we were trying to use. 

0:16:49.540 --> 0:16:57.20 
Lance 
So since we were on a on an on supported server using an unsupported version. 

0:16:57.860 --> 0:17:2.230 
Lance 
The the team, US and the folks at Seton decided. 

0:17:2.970 --> 0:17:5.420 
Lance 
Let's incrementally. 

0:17:6.340 --> 0:17:20.10 
Lance 
Uh, migrate this thing up. Let's go from 2010 on Prem to 2013 on Prem will go then to 2016 on Prem and then from 2016 will be able to use the free tools to go up to Azure. 

0:17:21.70 --> 0:17:22.360 
Lance 
OK, sounds great. 

0:17:23.160 --> 0:17:23.730 
Lance 
Uh. 

0:17:24.640 --> 0:17:34.270 
Lance 
Didn't exactly work that way, but we did get ourselves to 2013, so we're on a supported server on Prem running a supported application on Prem. 

0:17:35.240 --> 0:17:38.780 
Lance 
And we had 80 sync issues. 

0:17:39.700 --> 0:17:49.330 
Lance 
Which I think we've mostly got solved now and that's that's fresh. If you talk to us a week and 1/2 ago, they weren't solved. 

0:17:50.50 --> 0:17:51.320 
Lance 
They were still a poop shell. 

0:17:52.490 --> 0:17:53.900 
Lance 
So what's our plan? 

0:17:54.900 --> 0:17:55.950 
Lance 
Our plan is. 

0:17:57.870 --> 0:18:2.420 
Lance 
To use you guys, your group as our resellers mostly check. 

0:18:3.120 --> 0:18:7.310 
Lance 
Get SharePoint completely up and to Azure. 

0:18:8.150 --> 0:18:17.70 
Lance 
In order to do that, we have to have our our Active Directory from Prem synced up into Azure so we can manage those permissions. 

0:18:18.210 --> 0:18:41.840 
Lance 
Take that SharePoint application and you know get our permissions wrapped up around it. I got an auditing company. I want to come in and audit how we harden Azure. Since we're not up there at all and we don't have any data up there and get them to tell us all the terrible things that we're doing, engage with, you know, one of your groups to help us go and fix those permissions and and understand them and harden them. 

0:18:43.210 --> 0:18:44.340 
Lance 
Take a deep breath. 

0:18:45.230 --> 0:18:59.290 
Lance 
Relax for a couple of weeks and then take part of that SharePoint site and open it up to the greater Internet so we can do some file sharing with some clients because we have a need for that. 

0:19:1.260 --> 0:19:4.960 
Lance 
At that point I, Troy and I feel like we'll have hit a plateau. 

0:19:5.960 --> 0:19:29.90 
Lance 
We've got a little bit more of a cloud presence up there. We got a power BI that's up in Azure. We'll have this instance of SharePoint up in Azure. We'll have a little bit more of an idea of how to manage permissions for that. We'll have a reseller of our Microsoft product. So we've got a partner that's motivated to support us on learning how to use the environment. 

0:19:29.780 --> 0:19:41.200 
Lance 
Troy and and his, you know, the other guys, his peers does do a little bit more education on containerization and Microsoft's world and then sit down and say, OK. 

0:19:41.890 --> 0:19:46.80 
Lance 
Let's work with you guys and and map out a road map. 

0:19:46.750 --> 0:19:49.810 
Lance 
To get certain classes of our workers. 

0:19:51.50 --> 0:20:1.120 
Lance 
You know, up to some sort of a virtual desktop. Look at some of the options form some budgets around it and some timelines work with the management team here and say all right. 

0:20:2.100 --> 0:20:3.370 
Lance 
Virtualization. 

0:20:4.310 --> 0:20:5.600 
Lance 
Here's how we can do it. 

0:20:6.960 --> 0:20:9.340 
Lance 
Get some buy in from them and move forward. 

0:20:10.490 --> 0:20:16.630 
Lance 
That was a lot of words, but does that give you? Does that give you an idea of of your question of, you know, what we're hoping to do? 

0:20:17.630 --> 0:20:18.160 
Jerry Franks 
Very much. 

0:20:36.710 --> 0:20:36.870 
Lance 
But. 

0:20:17.490 --> 0:20:46.560 
Kirt Spaulding 
Uh, yes, from an IT like general IT strategy perspective, yes. And you know we we are recording this. So we do have a transcript, so no worries about the exceptional detail, OK. So we've got kind of this long term road map right from a SharePoint scope perspective. When we think about like the SharePoint strategy, we also have to consider. 

0:20:46.900 --> 0:20:52.910 
Kirt Spaulding 
Or what? What is our like desired future state for communication and collaboration within the org? 

0:21:0.510 --> 0:21:0.770 
Lance 
Ohh. 

0:20:53.370 --> 0:21:1.340 
Kirt Spaulding 
It I mean, we're we're in a teams meeting right now. Are you currently using teams like as your internal chat tool and and things like that? 

0:21:1.880 --> 0:21:5.50 
Lance 
No, we currently, I mean we have been. 

0:21:6.900 --> 0:21:9.770 
Lance 
An absolute Prem organization. 

0:21:10.990 --> 0:21:15.700 
Lance 
Just like a lot of other people, the pandemic really helped kick some doors open. 

0:21:16.420 --> 0:21:19.530 
Lance 
So currently we use Goto meeting to have meetings. 

0:21:20.710 --> 0:21:22.890 
Lance 
We use slack for chat. 

0:21:25.120 --> 0:21:25.560 
Lance 
And. 

0:21:26.960 --> 0:21:28.690 
Lance 
And that is. 

0:21:29.350 --> 0:21:31.400 
Lance 
Kind of the extent of it. 

0:21:32.280 --> 0:21:32.820 
Lance 
Umm. 

0:21:35.10 --> 0:22:0.190 
Lance 
Yeah, I think that's kind of the extent of it. And and just one other piece on us as as a organization, we have a call center. So we have about 120 people that are one class of individual. And then we've got our other side of our business and you know called the administrative side, that's a that's a separate class with a separate set of tools. We got about 120 people that are on RDS servers on Prem. 

0:22:0.940 --> 0:22:14.810 
Lance 
There were migrating up to a new cloud solution that somebody else's cloud solution that's not a Microsoft product. So it's a CRM dialing machine, the whole extravaganza. So proprietary product that they'll be up into. 

0:22:15.550 --> 0:22:23.570 
Lance 
What we're looking at at forming solutions for ultimately is our fifty or so administrative workers. 

0:22:24.570 --> 0:22:28.840 
Lance 
And they're the ones using slack for chat and go to meeting for meetings. 

0:22:30.80 --> 0:22:31.760 
Lance 
To Troy, did I leave anything out? 

0:22:32.680 --> 0:22:33.60 
Troy Heitmann (Guest) 
No. 

0:22:34.20 --> 0:22:34.250 
Lance 
OK. 

0:22:39.870 --> 0:22:40.200 
Lance 
No. 

0:22:36.350 --> 0:23:5.720 
Kirt Spaulding 
OK. And the the reason that's important is because within the Microsoft 365 cloud, everything everything's connected, right? You know, teams, teams is from Microsoft Vision and strategy standpoint teams is meant to be like the one stop shop. You know you can have your chat, your calendar, your meetings, your phone calls, your collaboration across different documents. You know accessing those power BI dashboards. 

0:23:32.220 --> 0:23:32.660 
Lance 
Yep. 

0:23:6.340 --> 0:23:32.700 
Kirt Spaulding 
All of those things. So if we're using, say, third party applications, you know, go to meeting and and slack for the meeting and chat functionalities. Decision has to be made. It's like hey, well, are we gonna leave that third party stuff in place and truly just focus on SharePoint online and that those capabilities are we going to adopt you know the full Microsoft 365 ecosystem and make. 

0:23:33.440 --> 0:23:36.450 
Kirt Spaulding 
Is that where we're headed? You know, like, long term, I mean. 

0:23:35.570 --> 0:23:40.420 
Lance 
That we're we're headed toward that decision junction, and I'm well aware of the decision. 

0:23:41.100 --> 0:23:41.730 
Kirt Spaulding 
OK. 

0:23:44.860 --> 0:23:45.880 
Troy Heitmann (Guest) 
It's a sales pitch. 

0:23:42.60 --> 0:23:46.50 
Lance 
It it it's I am well to be, to be blunt. 

0:23:46.920 --> 0:23:47.450 
Lance 
Umm. 

0:23:49.650 --> 0:23:50.430 
Lance 
Teams. 

0:23:51.460 --> 0:23:53.750 
Lance 
Once you're in teams, I think it works great. 

0:23:54.810 --> 0:24:7.260 
Lance 
But teams is a is a bit of a challenge when you're when you're not a teams user. Like right now my camera's not even working for this thing, but that's because I'm using so many different applications to use these peripherals and it just machine gets confused. 

0:24:8.530 --> 0:24:10.650 
Lance 
But I think the budget. 

0:24:11.420 --> 0:24:24.640 
Lance 
On when once we create once we can get to a stable area with SharePoint we we go ahead and develop a road map. We develop a cost and a budget. I think once you start to bundle all these Microsoft products in together. 

0:24:25.290 --> 0:24:27.630 
Lance 
That's why teams become so compelling. 

0:24:28.730 --> 0:24:32.100 
Lance 
So I our management team is not in love with teams. 

0:24:39.750 --> 0:24:40.170 
Kirt Spaulding 
Sure. 

0:24:32.960 --> 0:24:46.100 
Lance 
But I think they'll be in love with the total package price if that makes sense, and my goal would be to to be we've always been a Microsoft shop is to be completely in that Microsoft ecosystem. 

0:24:47.200 --> 0:24:49.640 
Lance 
But we're almost to the decision point. 

0:24:51.540 --> 0:24:52.80 
Lance 
Make another. 

0:24:55.400 --> 0:24:55.740 
Lance 
Yeah. 

0:25:2.540 --> 0:25:2.960 
Lance 
OK. 

0:24:51.300 --> 0:25:21.10 
Kirt Spaulding 
OK. Well, that's a it's a really important decision point because that's going to influence how you do your architecture as it relates to to SharePoint, right? If you're just so now we're talking about like the IT governance aspect of it and then there is that corporate governance aspect of how people are using the tools. But from the IT perspective say say in a scenario where like Nope, we're not using teams, we're sticking with slag zoom. 

0:25:22.200 --> 0:25:22.650 
Lance 
Whatever. 

0:25:21.130 --> 0:25:32.170 
Kirt Spaulding 
You know whatever. Well, uh the say for content like documents, files, resources, news, et cetera, not unstructured data. 

0:25:32.650 --> 0:26:5.140 
Kirt Spaulding 
Umm how how that is handled is different in a SharePoint only scenario versus a teams plus SharePoint scenario. And then there's also that wrinkle of OneDrive. There's kind of this document lifecycle right in the for Microsoft. You know I like to use me, we and us. So OneDrive, you know, that's where documents are born. That's like the me thing. It's got, you know, fully backup version control. I can share if that's enabled. And then when I'm ready to work on stuff with my colleagues that's where teams comes into play. 

0:26:5.280 --> 0:26:10.760 
Kirt Spaulding 
And on the SharePoint back end, when you have a team, uh, the uh. 

0:26:11.700 --> 0:26:43.70 
Kirt Spaulding 
Maybe not the control plane, but the control container is a Microsoft 365 group, so whenever I have a Microsoft 365 group that's automatically provisioning different resources, a SharePoint team site, a Microsoft team and then you can have other things like planners and stuff like that. So when we when we start to think about the Microsoft 365 groups, if we're not going to use teams and we don't want to use team sites at all. And typically team sites are not. 

0:26:44.30 --> 0:27:15.230 
Kirt Spaulding 
There there met for, containing like, uh, work in progress. And then you have what's known as SharePoint communication sites. So if you're used to the SharePoint Server model where everything is site, subsites and pages, they break it out differently in SharePoint online where they have what's known as a hub. Sites which might you might consider that like a home page or a portal page. But there's other design stuff going on with it and then communication sites, you know, a typical pattern there is that departments. 

0:27:15.380 --> 0:27:28.70 
Kirt Spaulding 
Or business units are going to have a communication site and that is where typically that's like a final resting place for complete documents and records. And you would control security. 

0:27:29.570 --> 0:27:39.550 
Kirt Spaulding 
Typically at that container level, um as a as a general best practice, because if you start to get down into like the document library, even folder level permissions. 

0:27:40.680 --> 0:27:48.160 
Kirt Spaulding 
It can get. It can get really hairy it really quick in terms of being able to keep things under control. 

0:27:48.500 --> 0:27:49.50 
Lance 
Fair enough. 

0:27:50.760 --> 0:27:56.210 
Kirt Spaulding 
So just to just to kind of wrap it back, so again that that key decision is. 

0:27:57.620 --> 0:28:27.130 
Kirt Spaulding 
Are we going to use teams? You know, as part of our our business operations that leads into the SharePoint governance conversation of, OK, how we're gonna set up our architecture to include communication sites and team sites. And then when it comes to migration, there's an order of operations there too. You want to migrate. Well, well one you would want to identify you know your data state essentially by, you know, sensitivity categories. 

0:28:27.280 --> 0:28:57.550 
Kirt Spaulding 
Whether it's public, internal, you know sensitive or, you know private or compliance related right determine you know what are going to be your most complex departments or business units to migrate and then your lease complex. And then ideally you start with those low hanging fruit to show be able to show progress be able to get people using the new tools because I mean as you kind of alluded to if you're using say multiple different tools like Slack or go to meeting and then you go to teams. 

0:28:57.790 --> 0:29:3.930 
Kirt Spaulding 
There there is a learning curve associated to being able to use that application, so you know. 

0:29:4.440 --> 0:29:11.350 
Lance 
We're we're we're running short on time for me. But I'm thank you very much. 

0:29:14.340 --> 0:29:15.0 
Lance 
That's. 

0:29:15.690 --> 0:29:19.930 
Lance 
OK, so here's what I think by by what you just said and I and I'm hearing you. 

0:29:21.610 --> 0:29:25.980 
Lance 
I think what we so I think I was. 

0:29:28.370 --> 0:29:31.530 
Lance 
I was off base by how we get to our next plateau. 

0:29:32.470 --> 0:29:41.10 
Lance 
I think how we get to our next plateau should be to get SharePoint up to 2016 on Prem. 

0:29:42.530 --> 0:29:43.480 
Lance 
And stop there. 

0:29:44.280 --> 0:29:51.590 
Lance 
Because the 2016 SharePoint on Prem can be used like the glorified file share we have today. 

0:29:53.160 --> 0:30:0.290 
Lance 
And hang on, Troy. And then I think we need to dive into, you know. 

0:30:1.170 --> 0:30:7.900 
Lance 
What is our our road map for getting, you know, for virtualizing this company in the Microsoft ecosystem? 

0:30:9.110 --> 0:30:13.840 
Lance 
What's it gonna cost to move through and what does that plan look like? 

0:30:14.710 --> 0:30:16.130 
Lance 
And you know. 

0:30:16.900 --> 0:30:25.990 
Lance 
Get the executive team to weigh in on is is that their? Is that their vision for the future and and I hope it is and I think you know, I'm gonna sell it. 

0:30:26.900 --> 0:30:34.830 
Lance 
Because I think that's where we need to go. And if it is, then when we migrate SharePoint up, you know, to your point. 

0:30:35.610 --> 0:30:39.650 
Lance 
We we govern it in a way that's going to make. 

0:30:40.350 --> 0:30:46.10 
Lance 
You know that's going to dovetail with those other products, you know, mainly OneDrive and teams. 

0:30:47.440 --> 0:30:53.880 
Lance 
If they decide they're not ready for something like that, then to go half *** up there. 

0:30:54.800 --> 0:31:0.560 
Lance 
Is is not going to be a very efficient way to live. Is. Is that a fair assessment of what? 

0:31:1.190 --> 0:31:3.750 
Lance 
What you were trying to communicate to me or or my off? 

0:31:4.390 --> 0:31:16.80 
Kirt Spaulding 
No, I I I think you're you're actually right on track in terms of you know just upgrading the 2016 if that's a maybe a something that can be easily done so that you can. 

0:31:17.280 --> 0:31:32.820 
Kirt Spaulding 
Say, maintain until some of these say higher level strategy discussions happen, that may be the best course of action for you because you're absolutely right. If you if you go into this without without like a plan and an understanding of how. 

0:31:33.400 --> 0:31:39.310 
Kirt Spaulding 
They like the the Microsoft 365 ecosystem is huge and there is. 

0:31:40.210 --> 0:31:52.20 
Kirt Spaulding 
A lot of considerations that need to need to happen and the executive team or whoever's driving, say like the Governance Board or whoever they need to be on board because ultimately it impacts. 

0:31:52.110 --> 0:31:52.490 
Lance 
Yeah. 

0:32:3.370 --> 0:32:3.740 
Lance 
Sure. 

0:31:52.120 --> 0:32:14.490 
Kirt Spaulding 
Umm, you know everyone in the organization now of course you can scope it to you mentioned like 50 users or using administrative workers. You can scope it down, but having that longer term, hey, we're gonna adopt, we're gonna move into the Microsoft 365 ecosystem and we're gonna accomplish. 

0:32:26.840 --> 0:32:27.90 
Lance 
Yeah. 

0:32:14.570 --> 0:32:46.500 
Kirt Spaulding 
You know, you know share sharepoint's going to control our content. It's going to have our news. We're gonna collaborate with teams. Everything's gonna be secure because we're gonna have E5 and purview, and it's all gonna be compliant cuz we get the audit. All of those types of questions you VCs needs to truly understand that aspect from a planning perspective before you really kind of kick off into the you know digital transformation into the cloud. 

0:32:47.250 --> 0:32:55.600 
Lance 
Area so who? So for me to get the executive team to do that, you know, fine Lance, how much? 

0:32:57.370 --> 0:33:11.140 
Lance 
What is it gonna cost us to maintain? And then what is what? It's gonna be the implementation cost. Who's my partner to help me, you know, to to help understand our business and help Troy and I. 

0:33:12.20 --> 0:33:15.800 
Lance 
Create a road map with an accompanying budget. 

0:33:19.330 --> 0:33:19.860 
Kirt Spaulding 
Ohh. 

0:33:19.150 --> 0:33:21.550 
Wayne Aune 
Yeah, that would be nice. It would be us. 

0:33:19.490 --> 0:33:21.980 
Jerry Franks 
I think I think Wayne, that's Scott it you're. 

0:33:23.960 --> 0:33:32.610 
Wayne Aune 
Yep, cause 'cause I'm bringing red level in as a tool. My tool belt obviously we needed that help and it's who's our. 

0:33:33.530 --> 0:33:37.170 
Wayne Aune 
Our partners got our our, my main company goes with. 

0:33:38.150 --> 0:33:38.780 
Wayne Aune 
So. 

0:33:40.410 --> 0:33:50.350 
Wayne Aune 
And then we have a company out at out in Boston called versatile and they are knee deep in this stuff too, but they don't even touch SharePoint. Nobody touches SharePoint except for red level. 

0:33:51.950 --> 0:33:52.160 
Lance 
But. 

0:33:51.270 --> 0:33:55.0 
Wayne Aune 
So as far as the big picture is concerned, then we we need to have a meeting like this. 

0:33:56.90 --> 0:33:57.90 
Wayne Aune 
To go over. 

0:33:58.270 --> 0:34:4.340 
Wayne Aune 
Your your vision cause obviously worked for all flows first, then then how do we support workflow and then? 

0:34:5.140 --> 0:34:16.680 
Wayne Aune 
Understanding what you can do with online tool sets, and that's where we would come in and say here's the possibilities you asking for help with Tim. 

0:34:18.240 --> 0:34:33.370 
Wayne Aune 
And we're kind of wait, I thought I'd wait till after this migration took place, but you you asked, what does it look like? What can we do? How can we do it? I think that meeting should come next. Then let's get you on the 13 or 16 and then let's let's explore. 

0:34:33.780 --> 0:34:40.620 
Lance 
That cause what I'm hearing now is it's not the right time to go up to Azure when we haven't formed that vision. 

0:34:42.940 --> 0:34:48.440 
Lance 
So let's let's let's get to a stable place with SharePoint. 

0:34:49.750 --> 0:34:57.610 
Lance 
And then let's let's start to learn and form the vision and I got, you know, I gotta give the the the executive team. 

0:34:58.340 --> 0:35:0.480 
Lance 
The the road map and the budget. 

0:35:1.380 --> 0:35:6.190 
Lance 
And so that they can, they can evaluate it and decide if they support that vision. 

0:35:6.940 --> 0:35:9.170 
Lance 
You know, we need to go more virtual, we know that. 

0:35:9.790 --> 0:35:10.370 
Lance 
But. 

0:35:12.340 --> 0:35:22.410 
Lance 
You know that that is our thing. So I mean, you know, Troy, Troy makes a good point is, is for us, we're going to need that. We're going to need a license that SharePoint 2016. 

0:35:23.850 --> 0:35:26.640 
Lance 
And and license it on Prem. 

0:35:27.980 --> 0:35:40.910 
Lance 
So I'm gonna need some help on on figuring that. I think that's was part of the impetus here is licensing it in Azure has has a more attractive model and I think we all focused on that. 

0:35:43.660 --> 0:35:45.800 
Lance 
So what? Yeah, I mean. 

0:35:46.930 --> 0:35:53.0 
Kirt Spaulding 
Well, how much? How much content in SharePoint are we talking about? And you know the? 

0:35:53.860 --> 0:36:4.320 
Kirt Spaulding 
The databases can. The data can almost be handled, say separately. Now I'm not familiar with how much of the server 2016 licenses would cost. 

0:36:5.490 --> 0:36:20.380 
Kirt Spaulding 
But from a if if it's a, you could potentially move your content over and then have a plan just for the SQL data, whether that's moving it into an Azure SQL database or establishing a data data gateway. 

0:36:21.370 --> 0:36:31.570 
Kirt Spaulding 
It's and again coming in with with minimal context, it's hard for me to tell you the the best path, but ultimately you are. You are right like. 

0:36:33.680 --> 0:36:54.180 
Kirt Spaulding 
Have a vision and a strategy that's based on what the business needs. That is what's going to sell to you know, the executives. I mean, of course, your security and compliance things are important, but then there's also the, you know, you've got these multiple third party apps you can highlight, you know, the inefficiencies that are caused by that, you know the. 

0:36:52.840 --> 0:37:7.610 
Lance 
Sure, I got. I got. Yeah. I'm. I'm sorry. I'm just. I I I'm. I apologize. But I I got a weird Friday where I've got a hard stop pretty quick. I I understand what you're saying. I'm not worried about making the case. 

0:37:8.350 --> 0:37:8.880 
Kirt Spaulding 
OK. 

0:37:8.400 --> 0:37:17.570 
Lance 
What I worried about is I'm stuck right now with, quite frankly, an unlicensed version of SharePoint. 

0:37:19.640 --> 0:37:27.620 
Lance 
And if I shouldn't go up to the cloud, I need to figure out what it looks like to properly license it to be on Prem. 

0:37:30.340 --> 0:37:51.220 
Lance 
And right now that's that's quite frankly in my mind right now, that's my overriding concern. This is the, you know, and I appreciate it. And I think you know what you're making a good case. And I I think you I appreciate you know the eye opening. This is the first time in a five month project that I've got. You shouldn't move up to SharePoint because you haven't figured out what you want to be when you grow up. 

0:37:52.780 --> 0:37:55.350 
Lance 
So I'm I'm kind of stuck right now. 

0:37:56.680 --> 0:37:57.550 
Lance 
Where I'm at. 

0:37:59.600 --> 0:38:0.60 
Kirt Spaulding 
I. 

0:37:59.380 --> 0:38:0.490 
Lance 
That makes some sense. 

0:38:0.850 --> 0:38:29.310 
Kirt Spaulding 
No, I I understand. And your your immediate, you know issue you know that that needs to be solved, right. You know we need need need some space to breathe before you can really you know dive into some of that other stuff. So I think that's clear we've we've captured it in the transcription. You know I'll make sure that that's available to Wayne and both you you and you and Troy and then I think additional conversations can be handled offline. 

0:38:29.640 --> 0:38:39.510 
Lance 
And and you your role in this in this group you're a third party company separate from from sighting true. 

0:38:40.650 --> 0:38:41.230 
Jerry Franks 
Correct. 

0:38:40.190 --> 0:38:42.340 
Wayne Aune 
Correct. Yep, Yep. 

0:38:40.560 --> 0:38:45.50 
Lance 
3rd off and and you guys, your expertise is actually. 

0:38:46.80 --> 0:38:48.530 
Lance 
Supporting making these large lifts. 

0:38:49.510 --> 0:38:50.860 
Lance 
To get up into the cloud. 

0:38:52.340 --> 0:38:53.890 
Lance 
That is that fair. 

0:38:55.660 --> 0:38:57.220 
Jerry Franks 
What? Yeah. 

0:38:58.240 --> 0:38:58.470 
Jerry Franks 
Yeah. 

0:38:55.620 --> 0:38:58.910 
Wayne Aune 
In our case, yes, it, like I said it big. 

0:38:57.780 --> 0:39:0.940 
Lance 
For us in my in my circumstance, what we would use you for. 

0:39:2.260 --> 0:39:2.570 
Lance 
OK. 

0:39:2.750 --> 0:39:3.40 
Wayne Aune 
Yep. 

0:39:3.630 --> 0:39:5.800 
Lance 
Cool. I just, you know, and that's great. That's awesome. 

0:39:6.990 --> 0:39:14.30 
Lance 
I just, you know, you get confused who all the players are in in everything that that you do in this, so I think. 

0:39:15.420 --> 0:39:27.200 
Lance 
Yeah, I think you've given me given us a bunch to think about. So. So when you've got somebody more appropriate to help us figure out our our licensing costs. 

0:39:27.870 --> 0:39:29.680 
Lance 
On the SharePoint decisions. 

0:39:30.560 --> 0:39:30.990 
Wayne Aune 
Yes, Sir. 

0:39:30.780 --> 0:39:36.590 
Lance 
And I and and to form this road map for going virtual. They're they're kind of two. 

0:39:37.760 --> 0:39:41.540 
Lance 
Separate tracks. Some you know the. 

0:39:42.730 --> 0:39:47.610 
Lance 
You know they crossover, but they're, but they're they're similar, but they're they are separate tracks. 

0:39:48.450 --> 0:39:49.890 
Lance 
Make does that make sense? 

0:39:52.400 --> 0:39:53.20 
Wayne Aune 
So get. 

0:39:51.170 --> 0:39:54.180 
Lance 
Alright, so we we need to put. Yeah, go ahead. 

0:39:54.530 --> 0:39:55.670 
Wayne Aune 
So. So kirt. 

0:39:57.650 --> 0:39:59.240 
Wayne Aune 
So we get him to 16. 

0:40:0.80 --> 0:40:13.90 
Wayne Aune 
Because the decision that did that they make is it is it gonna hinder you if they don't make a decision? Just say I I just want to get them up to up to the cloud. 

0:40:14.280 --> 0:40:32.310 
Wayne Aune 
Does that affect how much it would be? I'm looking for a budget number, so if I see I get him to 16 and then you get him up in the cloud. Just kind of a whole picture deal. Could you answer that yet or is that is that those decision needs to be make before you do anything? 

0:40:33.160 --> 0:40:38.110 
Jerry Franks 
Those decisions need to be made before. I mean ohh. I'm sorry. Is that for Lance or? 

0:40:38.660 --> 0:40:39.510 
Wayne Aune 
So for Kirt. 

0:40:39.460 --> 0:40:40.340 
Lance 
No you guys. 

0:40:39.370 --> 0:40:40.990 
Jerry Franks 
Or for Kirt. OK. 

0:40:42.690 --> 0:40:44.660 
Kirt Spaulding 
Just just to be clear. 

0:40:54.710 --> 0:40:54.960 
Wayne Aune 
What? 

0:40:45.900 --> 0:41:2.660 
Kirt Spaulding 
You're you're referring to like the strategic direction. Decisions like the the application strategy or which which decision because you know once they move the the purpose of the move to 2016 in this context is to you know. 

0:41:5.670 --> 0:41:6.80 
Wayne Aune 
Yep. 

0:41:8.640 --> 0:41:9.20 
Wayne Aune 
Yep. 

0:41:10.80 --> 0:41:10.510 
Wayne Aune 
Yes, Sir. 

0:41:3.520 --> 0:41:13.350 
Kirt Spaulding 
Basically, provide some breathing room because end of life and end of support is coming here and like a month and 1/2 and that's that's an issue in a regulated environment. 

0:41:13.890 --> 0:41:14.260 
Wayne Aune 
Yes, Sir. 

0:41:14.190 --> 0:41:18.70 
Lance 
It's coming to an end of it. Support is coming. For what? Ending for what? 

0:41:18.780 --> 0:41:19.320 
Troy Heitmann (Guest) 
SharePoint. 

0:41:18.870 --> 0:41:20.900 
Kirt Spaulding 
SharePoint Server 2013. 

0:41:21.590 --> 0:41:24.230 
Lance 
Right, OK, exactly, exactly. 

0:41:25.890 --> 0:41:26.340 
Lance 
So. 

0:41:25.350 --> 0:41:27.400 
Wayne Aune 
I was just trying to see if there's a big picture. 

0:41:26.130 --> 0:41:29.780 
Jerry Franks 
So the answer. So let me let me take a stab at your question, Wayne, so. 

0:41:59.430 --> 0:41:59.870 
Wayne Aune 
OK. 

0:41:31.210 --> 0:42:1.370 
Jerry Franks 
That's the thing. Stabilized. OK, then then take them to that next level. The way that red level would engage. Kirt, keep me honest here, but I think we would probably look at doing an initial discovery phase, which would be sort of a planning phase where we would dig in and then come up with the plan. And that's Lance, where we would be able to provide you the budget for you to move into the cloud in that full scoped out, you make the decision. This is what we want to do and then we'll give you the road map of how to get there. Am I going right? Would that, Kirt? 

0:42:1.450 --> 0:42:2.0 
Jerry Franks 
Keep me honest. 

0:42:16.630 --> 0:42:16.920 
Wayne Aune 
All right. 

0:42:23.750 --> 0:42:24.160 
Wayne Aune 
OK. 

0:42:2.590 --> 0:42:32.0 
Kirt Spaulding 
Yeah, that that. That's correct. That's typically how we manage engagements. You know, we'll have a single engagement for deeper business and technical discovery come up with a plan which includes preliminary design for things like the your content, communication, collaboration and data determining what's in scope and then the output of that is that you know we better understand your environment, your business and can you know provide a. 

0:42:32.90 --> 0:42:36.640 
Kirt Spaulding 
But that kind of road map that aligns with the business goals while also. 

0:42:40.710 --> 0:42:42.100 
Lance 
Yeah, but, but. 

0:42:36.440 --> 0:42:51.620 
Wayne Aune 
Yeah. No, I was just. I was just, I I get all that. I just wondering again, just trying to if I come back to Lance and say it's 30 freaking grand to get SharePoint on then then he might say ohh OK maybe we should move the cloud now. That's that's why I asked that but. 

0:42:51.540 --> 0:42:52.140 
Kirt Spaulding 
OK. 

0:42:52.100 --> 0:42:52.300 
Jerry Franks 
Yeah. 

0:42:51.560 --> 0:42:59.40 
Lance 
That's that's exactly it. I mean, because that's that was the one thing that that kind of pushed us toward cloud is. 

0:43:0.220 --> 0:43:0.810 
Wayne Aune 
The cost? 

0:42:59.880 --> 0:43:31.230 
Lance 
The IT, it seemed like Microsoft was making the on Prem obviously much less attractive economically than getting up into the cloud. So then we went in. Nobody brought this up as if you know, you really have to know where you're going. But you know, I we might economically need to dump that stuff up into the cloud and and create the rules to use it as a glorified file share while we spend the next several months. 

0:43:31.310 --> 0:43:34.690 
Lance 
Organizing a road map and then we're gonna have to redo those permissions. 

0:43:35.100 --> 0:43:36.250 
Wayne Aune 
Yep, that's. 

0:43:35.370 --> 0:43:46.260 
Lance 
I I just don't have any *** **** number, so I can figure this stuff out. Nor do I have a consistent, you know, set of advice on on here are your options. 

0:43:50.350 --> 0:43:50.630 
Jerry Franks 
Do you? 

0:43:47.150 --> 0:43:51.860 
Lance 
So you know the how, how do I, you know, what am I comparing right now? 

0:43:51.490 --> 0:44:1.590 
Jerry Franks 
Can we? Can we come back or with a, as they say, dump everything in an in an unorganized way up into SharePoint online? 

0:44:3.50 --> 0:44:3.480 
Kirt Spaulding 
Can't. 

0:44:5.700 --> 0:44:5.960 
Jerry Franks 
Yeah. 

0:44:22.880 --> 0:44:23.230 
Lance 
Well. 

0:44:4.160 --> 0:44:34.150 
Kirt Spaulding 
Can we? Yes. What? What? What's important is understanding how the the SQL data is being used and what those conflicts are. I mean, we could definitely take a look at like you know the assessment tool, but it's definitely an option. Like just get the content up there and sunset the server 2013. But in terms of like, yeah, figuring out those permissions, you don't have to do it all up front. You can kind of take it in an iterative process and it. 

0:44:34.250 --> 0:44:40.750 
Kirt Spaulding 
Is an iterative process anyway, but you know establishing what that MVP path is definitely. 

0:44:41.450 --> 0:45:7.230 
Kirt Spaulding 
It's an option. You know you don't. If you don't have have to have everything you know perfect and structured. Once it's in, you know, SharePoint online and you can just move, move your stuff over there. I can't, you know, tell you if that's, you know available because of your particular industry and requirements. But if that is an option, then yes, you could just do that and then fix it kind of in process later on to avoid that. 

0:45:8.470 --> 0:45:13.130 
Kirt Spaulding 
You know share server 2016 license chunk. 

0:45:13.940 --> 0:45:16.810 
Wayne Aune 
Can you yank them right out of 13 up up to the cloud? 

0:45:17.690 --> 0:45:25.620 
Kirt Spaulding 
Of for the most part, yes. But it's, uh, the data part that is the the hard part content and to an extent. 

0:45:26.720 --> 0:45:29.350 
Kirt Spaulding 
Like the the site designs and stuff. 

0:45:29.470 --> 0:45:37.780 
Kirt Spaulding 
Uh, but you. You'd have to take a look at what the migration assessment tool, which is free, kind of, spits out. 

0:45:37.0 --> 0:45:39.700 
Lance 
But what? OK, let's let's let's do this. 

0:45:40.410 --> 0:45:47.180 
Lance 
If we could cause your I you you know, and I like the fact that you can't really speak to it. 

0:45:48.190 --> 0:45:53.710 
Lance 
Seriously, unless you run your assessment tool that only makes sense. 

0:45:55.20 --> 0:46:9.70 
Lance 
You know, I I much rather you not talk out of your ear and I like the fact that you're not talking out of your ear. What do we need to do to run the assessment tool to give you something that you can look at and speak more intelligently to our situation. 

0:46:9.710 --> 0:46:17.210 
Lance 
Right. Is that? Is that what you're kind of getting at for you to for you to start to get serious about us you need to you need to assess the environment? 

0:46:18.860 --> 0:46:19.80 
Jerry Franks 
Yeah. 

0:46:20.730 --> 0:46:21.100 
Lance 
Cool. 

0:46:33.90 --> 0:46:33.510 
Lance 
OK. 

0:46:39.750 --> 0:46:40.160 
Lance 
Cool. 

0:46:18.150 --> 0:46:49.220 
Kirt Spaulding 
Yeah, ultimately that's that's how you know, engagements go right, understand the business requirements, understand those compliance or security needs or constraints. And then yeah, the assessing the technical environment, the migration assessment tool is free. Troy, I just posted it in the chat. If you just want to grab a link to it, but that'll give us an idea of what can't be migrated and then you need to go through a process. 

0:46:56.730 --> 0:46:57.180 
Lance 
Turn off. 

0:46:49.290 --> 0:47:4.250 
Kirt Spaulding 
Of OK determine what's actually critical and what can just be left behind. Right. You know you're moving houses, right? We don't get to bring everything. Like, get rid of the stuff that doesn't need to be there. And if it's critical and it can't be migrated, it has to be recreated. 

0:47:5.850 --> 0:47:7.530 
Wayne Aune 
All right, let's do that. 

0:47:5.920 --> 0:47:15.110 
Lance 
Perfect. Perfect. So I think that's a that's a concrete thing that that we should do to give you some some more ideas of just you know what we're running right now. 

0:47:16.480 --> 0:47:20.390 
Lance 
Who? Wayne in this? You know, in in this whole fabric. 

0:47:21.560 --> 0:47:25.450 
Lance 
Can get us a cost for the on Prem 2016 license. 

0:47:27.340 --> 0:47:33.200 
Lance 
And then can get us the cost again for this this Azure license if we move it up? 

0:47:34.100 --> 0:47:40.350 
Lance 
Because that the you know the delta between those two is is going to be a big influence in in what we do. 

0:47:41.830 --> 0:47:42.810 
Wayne Aune 
So I'll I'll take. 

0:47:41.610 --> 0:47:44.80 
Lance 
And if I remember correctly, it was pretty huge. 

0:47:53.140 --> 0:47:53.520 
Lance 
I like it. 

0:47:44.640 --> 0:47:59.580 
Wayne Aune 
So I I was thinking I I'd run with the on Prem and then have red level do their assessment and then advise us on licensing and I think we got licensing but let's let's let's keep that all with them. I'll take on Prem and. 

0:48:0.530 --> 0:48:0.920 
Jerry Franks 
So. 

0:48:0.480 --> 0:48:2.670 
Wayne Aune 
That way we have all their recipes. 

0:48:2.350 --> 0:48:2.960 
Lance 
Is that fair? 

0:48:3.520 --> 0:48:4.80 
Wayne Aune 
Pretty clean. 

0:48:10.800 --> 0:48:11.140 
Wayne Aune 
Yep. 

0:48:10.960 --> 0:48:11.270 
Lance 
Sure. 

0:48:3.370 --> 0:48:16.740 
Jerry Franks 
Yeah. So we're so we're clear, Kirt, at the tool is free. But for us to do the assessment part of it, we're gonna have to scope a little bit of project worked out for that, right. So we'll put, we'll put something together from that perspective and get that back to you. 

0:48:17.580 --> 0:48:18.920 
Lance 
That's that's fair enough. 

0:48:19.650 --> 0:48:27.310 
Lance 
Or no for, I mean you have a. Do you have a a feeling? Are we talking hundreds? Thousands for the scoping? 

0:48:29.680 --> 0:48:31.110 
Jerry Franks 
Heard. I'm thinking I mean. 

0:48:31.880 --> 0:48:33.730 
Jerry Franks 
Yeah. What, what? How many hours do you think? 

0:48:35.40 --> 0:48:35.610 
Lance 
That's better. 

0:48:34.470 --> 0:48:41.730 
Jerry Franks 
You know you're the you're the guy who's got to do the work and put time into it. So just rough guesstimate right now. Get rain, give estimate range. 

0:48:39.730 --> 0:48:43.90 
Lance 
You again pencil between us. Don't record this part. 

0:48:43.850 --> 0:48:45.100 
Lance 
I won't hold you to it. 

0:48:45.760 --> 0:48:46.190 
Kirt Spaulding 
OK. 

0:48:45.610 --> 0:48:46.310 
Wayne Aune 
You Nancy. 

0:48:46.390 --> 0:48:46.800 
Wayne Aune 
Sorry. 

0:48:46.910 --> 0:48:47.470 
Lance 
There it is. 

0:48:45.350 --> 0:48:48.440 
Jerry Franks 
Turn off the transcription, curt pretty good at this. 

0:48:48.510 --> 0:48:49.450 
Kirt Spaulding 
Uh. 
