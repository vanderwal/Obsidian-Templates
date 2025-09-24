---
title: "{{title}}"
subtitle: ""
author: <%=book.authors.map(author=>`\n  - ${author}`).join('')%>
publisher: "{{publisher}}"
cover_url: {{coverUrl}}
copyright: {{publishDate}}
isbn13: {{isbn13}}
isbn10: {{isbn10}}
date: {{DATE:YYYYMMDD}}
read-status:
tags: 
  - book
---
# {{title}}

Title: {{title}}
Author: <%=book.authors.map(author => `[[${author}]]`).join(', ')%>
ISBN: {{isbn13}}
Publisher: [[{{publisher}}]]
Copyright:  {{publishDate}}
Date: {{DATE:YYYYMMDD}}

![cover]({{coverUrl}})

Media Type: [[book]]

Book Note: [[{{title}} - Book Note]]