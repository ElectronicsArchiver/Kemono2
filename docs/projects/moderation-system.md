
# Moderation System

The moderation system gives certain users with the role <br>
of  `moderator`  the ability to perform supportive tasks.

The role is given by administrative users.

<br>

## Interfaces

```TypeScript
interface Action {
    
    categories : string []
    account_id : string
    type : string
    id : string
    
    /**
     *  A list of resource `id`s
     *  affected by the action.
     */
    
    entity_ids : string[]
    
    created_at : Date
    status : 'completed' | 'failed' | 'reverted'
}
```

<br>
<br>

## Process

### Moderator

<br>

1.  When the role of an account changes <br>
    to `moderator`, they are notified of this.
    
    <br>

2.  The account is henceforth able to access the `/mod` <br>
    endpoint, which leads to the moderator dashboard.

    On this page the they can see various <br>
    statistics, among them is the `tasks` list.

    <br>

3.  Each performed `task` results in an `action`.

<br>