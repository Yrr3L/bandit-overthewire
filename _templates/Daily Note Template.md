---
title: 📅 <% tp.date.now("YYYY-MM-DD") %>
created: <% tp.file.creation_date("YYYY-MM-DD") %>
modified: <% tp.file.last_modified_date("YYYY-MM-DD") %>
tags:
  - daily
  - note
category:
  - Notes
---
<< [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD').subtract(1, 'd').format('YYYY-MM-DD') %>|Yesterday]] | [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD').add(1, 'd').format('YYYY-MM-DD') %>|Tomorrow]] >>

> [!multi-column]
> 
>>[!todo]+ Due Today 
>>```tasks
>> not done
>> due <% tp.file.title %>
>> sort by priority
>> hide due date
>> ```
>
>> [!danger]+ Overdue
>> ```tasks 
>> not done 
>> due before <% tp.file.title %>
>> sort by priority
>> hide due date
>> ```
>
>> [!success]+ Completed
>> ```tasks
>> done <% tp.file.title %>
>> hide done date
>> ```

[[Calendar View]]
## New Tasks
