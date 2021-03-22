# Welcome to my blog

This is my first blog, and I am using it to explore how to use github pages. I am also using it as an exercise in Markdown.

I am demonstrating that I know how to make text **bold**, _italic_ and ~~in strikethrough~~. Markdown is really exciting because, in the words of Joseph Edwards:
> You can do loads of cool stuff with it.

It can also keep track of things I need to do:

- [x] Wake up
- [x] Get breakfast
- [x] Have a shower
- [ ] Go to the shops

I can't wait to do some more cool things.

## Posts

<ul  style = "margin-left:0;list-style:none">
    {% for post in site.posts %}
        <li>
            <span style = "font-size:14px;color:#828282">{{ post.date | date_to_long_string: "ordinal" }}</span>
            <h3>
                <a href="{{ post.url | absolute_url}}">{{ post.title }}</a>
            </h3>
        </li>
    {% endfor %}
</ul>
