A social media app for those that want to view polls and engage in educated debates. 
Each post is a poll that users can answer, view other people's answers, view debates that are happening/happened and even participate as jurors. 

## Features
### Polls
This is the core mechanic around which the app is built. Any user can add a poll. A poll will have a background image that is supplied by us or by the user (or AI generated), a question with two answers (.e.g Who will win? Trump/Bidome) and tags to classify the poll.

The feed for the users will be a bottomless scroll. Each poll will be an entire page, with a few components:

- Who made the post
- The poll question
- The poll results
- A debate replay
- A button to get additional context for the discussion
- A footer with a few options, like 'Profile', 'Home' and 'Add poll'

![[Pasted image 20231120211404.png]]

### Debates
Now we're getting into the meat and potatoes of what is going to be the hook and main method of interaction for the users. There will be a debate per X amount of answers in a poll, say one debate per 1000 answers. Upon choosing to enter a debate, the user will be placed into a room while waiting for 3 others to join. In the meantime, the user can still scroll through other debates/polls. Users can subscribe to some maximum limit, and if a debate room hasn't opened after X hours the user will be auto dequeued.

After enough people will be found, a room will open and then a debate will begin. Once a user needs to respond, they will get a notification and then X amount of hours to get in to respond. Once they open the app they will be time limited to respond. If they don't respond in time they will get kicked/penalized and their teammate will get an additional opportunity to answer. If both are AFK then they win by technicality. 

### Jury
Once a debate is finished, users who voted will get a notification that they have been selected as 'Jurors'. They and a few others can then adjudicate on the debate, and if any change their opinions (their initial votes) the debate will have some weight. Then after taking into account the adjudications of the debates will then affect the results of the poll (will be clearly marked!)

### Reward systems
ELO increases with convincing debates / Quests (tasks) like "be a juror 3 times", "convince 3 jurors of a different opinion", etc.
In app currency for cosmetics/customizables/themes. Grind for premium? Crypto?

### Premium
Queue priority, reduced debate limits

### Profile
User can grind to get badges and cosmetics(?). In the user profile, we'll have a spider graph representing them and their leanings (politics, open mindedness, etc...). 

### Search
Can search via tags or text and will get the hottest polls relevant to their search


## Generic
Build detailed user profiles in order to feed more relevant polls to them. Then display it in a neat format to show the user's interests and biases (i.e. user likes hardware, prefers amd over intel, likes football, prefers barcelona over madrid)

2FA + captcha will probably block most bots for a while at least. 

voice notes? - like whatsapp 

## Monetization
- Selling the results of the polls
- Letting companies post their own polls
- Premium - Algorithm prioritizes your polls

## Names
- Pollit
- SnapPoll
- SnaPoll

## Target audience
- Fandoms

## Jumpstart
- Initial traffic with bots/Indians/cheap internet traffic

## Distinction
- Gamefictation
- Debate

The poll is the basis for debating. Then you choose two of one opinion and two of the other opinion and N jurors. Jurors can then listen to the arguments an decide.

#TODO Cloud function 