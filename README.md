# All Types
There's a newly added types according to the comments in Paul's Powerpoint, which leads to total **35** different types showing as following.  
Please click [UX_Updates.pdf](./Updates_of_notifications.pdf) to see Paul's comments.  
Please also click [Cards Effects](./CARDTYPES.md) to see the effect based on the latest comments.  
<small>*__NOTE: Some updates haven't been synchornized to UXpin. Thus for final effect, please refer to this Markdown__*</small>

### Types list
- Profile
    - follow
    - profile_liked
    - profile_viewed
    - profile_shared
- Comment
    - comment_liked
    - comment_replied
    - comment_mentioned
- Post
    - post_mentioned
    - post_liked
    - post_shared
    - post_commented
- Newsfeed
    - newsfeed_post
    - newsfeed_mentioned
- Opportunity
    - opportunity
    - opportunity_recommended
    - opportunity_applied
    - opportunity_expiring
- Application
    - application_expiring
    - application_viewed
    - application_accepted
- Paid Services
    - payment
    - advertisement_outbid
    - advertisement_won
    - advertisement_viewed
    - advertisement_expiring
    - membership_actived
    - membership_expiring
    - membership_expired (TBC)
    - translation_received
    - translation_ongoing
    - translation_complete
- Other
    - reference_wrote
    - birthday
    - experience_wall
    - connection_applying
    - report_advise

## Data Structure
### Request
```javascript
    {
        api: '/Updates',
        method: 'POST',
        params: {
            timestamp: Date.now()
        }
    }
```

### Response
```javascript
    {
        "200": [
            {
                _id: "5ad44384fc3aa40c5a54cb90",
                from_member: "5ad44384ce31fdad2514d216",
                to_member: "5ad44384643b6df76db35d12",
                time: 496852839670,
                event_type: "<event_type>",
                feed_type: "5ad443afd6b8d3acade3821d",
                comment_id: "5ad443afe47badd7045eaaf7",
                post_id: "5ad443af923bf7b731eaea1d",
                seen: false
            }
        ]
    }
```

