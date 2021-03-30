# DTU Times Public API

## Setup

## Routes

* ### Story
    #### Example:
    > https://api.dtutimes.com/v1/story

    ### Parameters
    Parameter | Description
    --- | --- 
    {slug} | unique slug of the story


    #### Return value

    Field | Description
    --- | --- 
    id | Unique id of story
    title | title of the story
     biliner | two lines on the topic of story
     slug | slug used in the url
     views | numver of views
     status | status of publication
     imgUrl |  link of image used
     created_at | array of dates and timezone of creation
     updated_at | array of dates and timezone of updation
     published_at | date of publicition
     category | array containing details about the story
     user | array containing details about the author (user)
    
     
* ### Editions
    #### Example:
    > https://api.dtutimes.com/v1/edition
    #### Return value
    Field | Description
    --- | --- 
    *Still* | `renders`
    1 | 2 


* ### Instagram
    #### Example:
    > https://api.dtutimes.com/v1/instagram
    #### Return value
    Field | Description
    --- | --- 
    *Still* | `renders`
    1 | 2 



* ### Facebook
    #### Example:
    > https://api.dtutimes.com/v1/facebook
    #### Return value
    Field | Description
    --- | --- 
    fan_count | Number of followers
    category | Account category
    description | 
    cover |
    emails |
    id | 
    link |
    location |
    name |
    website |

* ### Device
    #### Example:
    > https://api.dtutimes.com/v1/device
    #### Return value
    Field | Description
    --- | --- 
    *Still* | `renders`
    1 | 2 



* ### Subscriber
    #### Example:
    > https://api.dtutimes.com/v1/subscriber

    ### Parameters
    Parameter | Description
    --- | --- 
    page | Page number of the subscribers  


    #### Return value

    Field | Description
    --- | --- 
    current_page | Current Page of the subscriber (Default is 1) 
    data | An array of objects of type Subscriber
    first_page_url | Url to the first page of subscribers
    from | Index of first subscriber
    last_page | Last page number of Subscribers
    last_page_url | URL of last page
    path | Path of the API
    per_page | Subscriber count per page
    prev_page_url | URL of previous page
    to | Index of last subscriber
    total | Total subscriber count

    ### Subscriber Object


    Field | Description
    --- | --- 
    id | Id of the Subscriber
    uuid | 
    email | Email of the subscriber
    sent_count | 
    open_count |
    created_at | Creation date of Subscriber
    updated_at | Last updated date of subscriber


* ### Notification
    #### Example:
    > https://api.dtutimes.com/v1/notification
    #### Return value:
    An array of notification objects
    Field | Description
    --- | --- 
    name | Name of notification 
    description | Description of Notification
    created_at | Date of creation
    link | Link of notification
