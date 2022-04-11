# Word count dashboard for a Ghost blog

## Backstory
The full story: [Visualizing my writing goals with live stats](https://www.growinginpublic.com/visualizing-writing-goals-live-stats/)

## About
This is a simple dashboard that shows the post count and word count in a Ghost blog over the past week, and all time.

It does this by reading in the posts from a Ghost blog using the Ghost API.

## To make this dashboard work for your blog
_A version of these instructions is also present in the UI itself, as you'll see when you load in the app code into Retool._

In Ghost:
1. First, you must be on at least the Creator plan, if you're using a hosted Ghost blog, to get API access.
2. Follow the instructions in the [Ghost API docs](https://ghost.org/docs/content-api/#authentication) to get a Content API key.

In Retool:
3. Download the Retool app file from this directory. Upload it into your Retool instance using the "Create new" => "From JSON" option.
4. Plug that API key into the `get_posts` Query in this Retool app. Replace the `YOUR-CONTENT-API-KEY-HERE` text.
5. Also, replace the `YOUR-URL-HERE` in the `get_posts` Query with the URL of your Ghost blog.
6. Finally, delete the instructions block from the UI. :)
