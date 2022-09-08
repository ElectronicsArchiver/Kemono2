
# File Upload

<br>

## Interfaces

```TypeScript
interface ManualUpload {}
```

<br>
<br>

## Process

<br>

1.  The account goes to `/posts/upload`

2.  Uploads the file

3.  The file gets processed

4.  The file gets sent for review to a moderator

5.  The moderator then decides to discard <br>
    the upload or approve for public view

<br>
<br>

## Issues

<br>

-   What happens when one mod approves <br>
    a file while the other one discards it?

<br>

-   Unlike DMs the file verification can take very <br>
    variable amount of time, so there should be <br>
    separate states for a given upload, like:
    
    -   `approved`
    
    -   `rejected`
    
    -   `pending`

<br>
