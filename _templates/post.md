<%*
const title = await tp.system.prompt("Post title");
const date = tp.date.now("YYYY-MM-DD");
const filename = date + "-" + title.toLowerCase().replace(/ /g, "-");
await tp.file.rename(filename);
-%>
---
layout: post
title: "<% tp.file.title %>"
date: <% tp.date.now("YYYY-MM-DD") %>
tags: []
---