# Time

> Foxfire is currently chilling out in Mbabane. She did an awesome google search to find out something special. We've got hold of the search url. Now at what time did she search?
>
> Flag format: CTF{yyyy-mm-dd-HH}
> 
> https://www.google.com/search?q=ectf+nitk&sxsrf=APq-WBucQC97ty5WJujCZdH3xgNKkG4DcA%3A1646337798523&source=hp&ei=Bh8hYqykHc64mAXkkoTgCg&iflsig=AHkkrS4AAAAAYiEtFvYpL6BEakDJQ-fOP-eWa7kvFyAO&ved=0ahUKEwisv6Kd3qr2AhVOHKYKHWQJAawQ4dUDCAg&uact=5&oq=ectf+nitk&gs_lcp=Cgdnd3Mtd2l6EAMyBAgjECcyBAgjECc6BAgAEEM6CwguEMcBEK8BEJECOgoILhDHARCvARBDOgUIABCRAjoLCAAQgAQQsQMQgwE6CAgAEIAEELEDOgcIABCxAxBDOhAIABCABBCHAhCxAxCDARAUOgUIABCABDoGCAAQFhAeOggIABAWEAoQHlAAWMMKYPUNaABwAHgAgAHcAYgBqgySAQUwLjcuMpgBAKABAQ&sclient=gws-wiz

The query contains many parameters, like `ei` which contains a timestamp. Unfurl the link wih [this tool](https://dfir.blog/unfurl/) to get the timestamp in GMT. Mbabane's timezone is +2 GMT.

The flag is `CTF{2022-03-03-22}`.
