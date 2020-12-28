![[Coding/mangadex-simplified/README]]

As mentioned in the readme the goal of this project was to take the html data from mangadex's frontpage and extract only the latest chapters from it. (As highlighted in the following image)
![[targetData.png]]

By commit ![[Coding/mangadex-simplified/Commit Log#0fbf08962cc95b5ba4854802a62015851a2fe5bd | 0fbf089]] I had managed to implement this such that I can close the project as a success
![[receivedData.png]]

Commits [[Coding/mangadex-simplified/Commit Log#d2ba34c16b8613163e3fe403c9feb3a317293153 | d2ba34c]] and [[Coding/mangadex-simplified/Commit Log#9b2c2e0d30cf2312c0edee0c3062112e16d940c3 | 9b2c2e0]] were edits to the readme file for formatting

Commit [[Coding/mangadex-simplified/Commit Log#f1639219223532585c9206bc7bf962827a21fb93 | f163921]] was some comment clarification

# Reflections
There is a line of code in main.py that goes like:
```python
titles = soup.select('.col-md-6.border-bottom.p-2 .manga_title.text-truncate')
```
I hope to remember the selection text especially when there is a class name that has spaces.
Note that `.col-md-6.border-bottom.p-2` has multiple `.`'s, this is a case where the class name has spaces. The way to get a proper selection is to replace all spaces with a `.`. This way you will get a proper selection instead of nothing.

