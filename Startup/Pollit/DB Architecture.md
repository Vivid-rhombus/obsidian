## Collections
What collections do we have:
- Users
- Polls
- Debates
- Store Items
- Shared customizables
- Topics (tags)
- Reports
- Badges
- Stats

Topic
```JSON
{
	"name": "string",
	"isMeta": bool
}
```

User
```JSON
{
	"name": "string",
	"bio": "string",
	"gender": "string",
	"profilePicUrl": "string",
	"dateOfBirth": date,
	"topicsOfIntrest": [
		{
			"_id": "string",
			"name": "string"
		}
	],
	"debateELO": number,
	"juryELO": number,
	"joined": date,
	"followers": [userId],
	"following": [userId],
	"myPolls": [pollId],
	"sharedPolls": [pollId],
	"recentPollHistory": [pollId],
	"debatesWon": [debateId],
	"participatedDebates": [debateId],
	"stats": {numbers},
	"badges": [badgeId]
}
```

Polls:
```JSON
{
	"creator": userId,
	"topics": [topicId],
	"title": "string",
	"options": {
		"optionA": {
			"title": "string",
			"totalVotes": number
		},
		"optionB": {
			"title": "string",
			"totalVotes": number
		}
	},
	"votes": subcollection({"userId": votedOption}),
	"backgroundUrl": "string",
	"debates": [debateId],
	"expiryDate": date,
	"createdAt": date
}
```

Debate
```JSON
{
	"status": "string",
	"poll": pollId,
	"participants": {
		"userId": {
			"votes": number,
			"chosenOption": "string",
			"gainedELO": number,
			"userImageUrl": "string"
		}
	},
	"jurors": {
		"userId": {
			"chosenUser": userId,
		}
	},
	"turns": [{"userId": userId, "message": "string"}],
	"turnIndex": number,
	"winner": "string",
	"mvp": userId
}
```