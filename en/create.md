---
layout: page
title: Create topic or event activity
permalink: /create/
button: true
ref: create
lang: en
published: true
---
Adding a topic or event

Copy an existing post in the  `_posts` directory to get started. Delete the specific details and leave empty (blank) the parts that you cannot specify. To create a topic you'll leave empty lines after the date and time lines. You can leave other lines empty too: location, sponsor, organizer, etc.

Relabel your file, keeping the .md ending. Add your .md file into the `_posts` directory. The post file name must be in the following format, so if it's a topic, choose a date several weeks or months in the future:

{% highlight markdown%}
YYYY-MM-DD-title.md
# Example 2017-01-02-Hot-Topic-Right-After-New-Year.md
{% endhighlight %}

# Config for posts
{% highlight markdown%}
---
# leave this alone
layout: post

# Whats the title of your event.
title:  "Talk on ES6 JavaScript"

# Url to your cover photo for your event. [optional - default will be used if not given]cover: "https://frontendmasters.com/assets/es6-logo.png"

#The date of the event.
date:   2016-02-01 16:04:19 +0000

#Start time of the event
start_time: "12:00"

#end time of the event
end_time: "13:00"

#event organizer details

#event organizer details
organizer: "Paul Cuciureanu"

#Make sure you setup your Organiser details in the _data directory in the community.yml file

---
{% endhighlight %}

## Post content

After you have setup your config, all you need to do now is write your content using markdown.

## Example Post

{% highlight markdown%}
---
layout: post

#event information
title:  "ReactJS"
cover: "http://blog.addthiscdn.com/wp-content/uploads/2014/11/addthis-react-flux-javascript-scaling.png"
date:   2016-03-28
start_time: "12:00"
end_time: "13:00"

#event organizer details
organizer_email: "david.boyne@test.com"
organizer_name : "David Boyne"
organizer_photo: "https://pbs.twimg.com/profile_images/660943257795457030/igA_joVD.jpg"

---

I will be doing a small talk on an Introduction into ReactJS. We will cover the following:

- What is React?
- How to get setup with React.
- How to get building React Apps.
- Bundle your application
- Release your application

If this sounds interesting please register your interest below.


{% endhighlight %}

## Thats all folks
Thats all you need to do. Once the website is built again using `jekyll build` or `jekyll serve` your new event will be shown.