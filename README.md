
This volt has a basic skeleton for Daily, Weekly, Monthly and Yearly periodict notes with goals and conclusions that are shared between the files.



Plugins:
1. Periodic Notes *by Liam Cain*
	- Turn off built-in Daily-notes plugin
1. Templater *by SilentVoid*
	- Turn on "Trigger Templater on new file creation"
	- Turn on "Automatic jump to cursor"
2. (Optional but recomended) Natural Language Dates *by Argentina Ortega Sainz*
3. (Optional but recomended) Calendar *by Liam Cain*




```
<% moment(tp.file.title, 'YYYY-MM-DD').format("YYYY-MM-DD")%>#<% moment(tp.file.title, 'YYYY-MM-DD').format("dddd DD/MM/YY") %>
```

## How does it work
This template uses 3 concepts to work:
- Obsidian embed file, or in our case, embed another note ([official docs](https://help.obsidian.md/How+to/Embed+files))
	- If you add `!` at the beginning of a link, it creates an embed of that reasurce. Example:
		- `[[2022-09]]` creates a link to september file
		- `![[2022-09]]` creates a embed so I can read the september file directly
- Obsidian Link to heading ([official docs](https://help.obsidian.md/How+to/Internal+link#Link+to+headings))
	- Embeding puts the entire file, but if we just one the goal, we can link to the title. Examle:
		- `![[2022-09]]` prints entire file
		- `![[2022-09#goal]]` prints only the september goal
- Templater's ability to read the document title and integration with MomentJS

## Templater and MomentJS

## Use the calendar to move accross daily notes
Once the plugin is installed, the calendar tab is hidden in the right pannel:

![5-weeks-months](https://github.com/Antoine-lb/obsidian-periodic-notes-sample/blob/master/screenshots/reveal-calendar.jpg?raw=true)

![5-weeks-months](https://github.com/Antoine-lb/obsidian-periodic-notes-sample/blob/master/screenshots/full-calendar.jpg?raw=true)

Read more about it here: https://github.com/liamcain/obsidian-calendar-plugin


## Why 5 weeks per month?
Because not all months start on monday and end in sunday.


![5-weeks-months](https://github.com/Antoine-lb/obsidian-periodic-notes-sample/blob/master/screenshots/5-week-months.jpg?raw=true)


![[https://github.com/Antoine-lb/obsidian-periodic-notes-sample/blob/master/screenshots/5-week-months.jpg]]

