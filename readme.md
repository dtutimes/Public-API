# DTU Times Public API

## Setup

## Routes

* ### Index
    #### Example:
    > https://api.dtutimes.com/v1
  
    #### Return value

    Field | Description
    --- | --- 
    id | Unique id
    title | title of the post
    biliner | two lines on the topic of post
    slug | unique keyword
    views | number of views
    status | status of publication
    imgUrl |  url of the image 
    created_at | array of dates and timezone of creation
    updated_at | array of dates and timezone of updation
    published_at | date of publicition
    category | array containing details about the post
    user | array containing details about the author (user)


* ### Story
    #### Example:
    > https://api.dtutimes.com/v1/story
    ### Specific keywords
    keywords | Description
    --- | --- 
    {slug} | details about the specific story


    #### Return value

    Field | Description
    --- | --- 
    id | Unique id of story
    title | title of the story
    biliner | two lines on the topic of story
    slug | unique keyword
    views | number of views
    status | status of publication
    imgUrl |  link of image used
    created_at | array of dates and timezone of creation
    updated_at | array of dates and timezone of updation
    published_at | date of publicition
    category | array containing details about the story
    user | array containing details about the author (user)
     
     
* ### Category
    #### Example:
    > https://api.dtutimes.com/v1/category
    ### Specific keywords
    keywords | Description
    --- | --- 
    {id} | details about the unique category


    #### Return value

    Field | Description
    --- | --- 
    id | Unique id
    name | Type of category
    slug | unique keyword
    created_at | date of creation
    updated_at | date of updation
    
    
* ### Gallery
    #### Example:
    > https://api.dtutimes.com/v1/gallery
    ### Specific keywords
    keywords | Description
    --- | --- 
    {slug} | details about the selected gallery


    #### Return value

    Field | Description
    --- | --- 
    name | Type of category
    biliner | two lines on the topic of story
    slug | unique keyword
    album_id | 
    status | status of publicition
    album_imgUrl | url of album cover page image
 
 
 * ### Society
    #### Example:
    > https://api.dtutimes.com/v1/society
    ### Specific keywords
    keywords | Description
    {slug} | details about the society
    {slug}/news | news about the selected society 
    {slug}/gallery | gallery details of the selected society


    #### Return value

    Field | Description
    --- | --- 
    id | Unique id of the user
    name | name of the user
    category | category type of the society
    slug | unique keyword of the society
    uuid | universal unique id
    user_id | unique society id
    status | status of publicition
    decription | description about the society
    linkedin | linkedin url of society head
    facebook | facebook url of society head
    instagram | instagram url of society head
    contact_mail | mail of the society head
    head_incharge | name of the society head
    pr_incharge | name of the PR incharge
    pr_contact_number | contact number of the PR
    head_contact_number | contact number of the head
    website | url of the society website
    referrals | number of referrals
    views | number of views
    society_imgUrl | url of society image
    
 * ### News
    #### Example:
    > https://api.dtutimes.com/v1/news
   
    #### Return value

    Field | Description
    --- | --- 
    id | Unique id of news
    title | title of the news
    uuid | universal unique id
    society_id | unique id of society
    status | status of publication
    description | description about the news
    view | number of views
    created_at | date of creation
    updated_at | date of updation
    imgUrl |  link of image used
    society | object containing details about the society and the society news
    media | array of objects describing about the media 
    
* ### User
    #### Example:
    > https://api.dtutimes.com/v1/user
    ### Specific keywords
    keywords | Description
    --- | --- 
    {id} | unique id of the user


    #### Return value

    Field | Description
    --- | --- 
    id | Unique id of the user
    name | name of the user
    uuid | universal unique id
    email | email address of the user
    username | username of the user
    activated | status of activation
    bio | User bio
    data_of_birth | date of birth of user
    linkedin | linkedin url of user
    facebook | facebook url of user
    instagram | instagram url of user
    display_mail | email address of the user
    email_verified_at |
    created_at | date of creation
    updated_at | date of updation
    blocked | status of blocked
    show | status of visibility
    position | position held by the user
    userImg | image url of the user photo
    media | media details about the user


* ### Editions
    #### Example:
    > https://api.dtutimes.com/v1/edition
    #### Return value
    An array of Edition Objects
    Field | Description
    --- | --- 
    id | Id of edition
    name | Edition Name
    link | Link of edition pdf
    ajax | 
    deleted_at | Deletion date of edition (Null if not deleted)
    created_at | Creation date of edition
    updated_at | Updation date of edition
    Period | Period of the edition
    sID | 
    imgUrl | COver Page of edition
    media | An array of **Media Objects**
    
    ### Media Object
    Field | Description
    --- | --- 
    id | Id of the media
    model_type | 
    model_id | 
    collection_name | Name of the collection
    name | Media Name
    file_name | Name of the file
    mime_type | tyoe of media
    disk | Public/Private
    size | Size of the media
    manipulations | 
    custom_properties | 
    responsive_images | 
    order_column |
    created_at | Creation date of media
    updated_at | Updation date of media

    > You can also get specific post by providing its id.( For example: https://api.dtutimes.com/v1/edition/61 )

* ### Facebook
    #### Example:
    > https://api.dtutimes.com/v1/facebook
    #### Return value
    Field | Description
    --- | --- 
    fan_count | Number of followers
    category | Account category
    description | Account Description
    cover | Cover photo and other details
    emails | Email Ids with the account
    id | ID of the account
    link | Link of facebook page 
    location | Precise location of DTU times
    name | Name of Account
    website | DTU times official website

* ### Facebook Posts
    #### Example:
    > https://api.dtutimes.com/v1/facebook/post
    #### Return value
    Field | Description
    --- | --- 
    created_time | Details of creation of post
    full_picture | Link of picture of the post
    message | message included in the post
    status_type | Status of the post
    permalink_url | Facebook Post link
    id | Id of the post
    
    > You can also get specific post by providing its id.( For example: https://api.dtutimes.com/v1/facebook/post/145561028808040_4347191505311617 )
    
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
