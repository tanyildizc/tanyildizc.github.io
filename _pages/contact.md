---
title: contact
description: "email is the best way to get in touch."
permalink: /contact
--- 



**{{ site.email }}**

<div class="tag-list copy-buttons">

<button class="btn btn-default" onclick="copyEmailtoClipboard('{{site.email}}')">copy address</button>

<a href="mailto:{{site.email}}">send email</a>
</div>

[rss](/rss) is the best way to follow me.

<script>

// copy email to clipboard

function copyEmailtoClipboard() {
    navigator.clipboard.writeText((arguments[0]));
}

</script>
