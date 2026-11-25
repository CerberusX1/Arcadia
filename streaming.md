---
layout: default
title: Streaming
---

# Streaming

Anyone is welcome to stream and use the Arcadia Discord for their streams.

---

## Our Streamers

{% if site.data.streamers and site.data.streamers.size > 0 %}
| Streamer | Platform | Streams |
|---|---|---|
{% for s in site.data.streamers %}| [{{ s.name }}]({{ s.url }}) | {{ s.platform }} | {{ s.streams }} |
{% endfor %}
{% else %}
No streamers are listed yet. Want to be the first? See [how to get listed](#getting-listed-and-announced) below.
{% endif %}

---

## Streaming Guidelines

1. If you see someone actively using the streaming channel while they are streaming, please do not join the channel and start making loud noises or trying to cause issues for the streamer.
2. Anyone is welcome to stream and use this Discord for their streams. This includes the ability to announce that they are streaming and to let others know whether or not the stream is open for anyone to join.
3. To announce streams you must have a streamer tag. To get a streamer tag, please send Sky a message on the [Discord](https://discord.gg/3UaP8ssBSv).

The [community rules]({{ '/rules/' | relative_url }}) apply to everything on the streams and in the Discord. Not following them will result in removal from the streams and the Discord.

---

## Getting Listed and Announced

To be added to the automatic go-live announcements and to the list above:

1. Read the streaming guidelines above and the [community rules]({{ '/rules/' | relative_url }}).
2. Send Sky a message on the [Discord](https://discord.gg/3UaP8ssBSv) to request a **streamer tag**, and include a link to your channel so you can be listed on this page.
3. Once you have the tag, you can announce your streams and let others know whether or not your stream is open for anyone to join.
