## All the usefull tips here

- ###  To search and delete node modules from older project.
#### we all suddenly face problem with device space getting full, main culprit for us developers is dependencies (node_modules), it can be more than 300MB+ 😲 for react and more if you add more dependencies later on, which we all do 🤦‍♂️.
#### There is a awesome tool to kill them, i mean not really kill but delete.
#### **[npkill](https://npkill.js.org/)** is just awesome easy to use cli tool.

- #### You can install globally by running 
```
$ npm i -g npkill
```
> #### Make sure you have node installed 

- #### You can also use it without installing it by running
```
$ npx npkill
```
<p align="center">
  <img src="https://npkill.js.org/img/start%20search.gif" width="450px" title="start search" alt="npkill searching">
  <img src="https://npkill.js.org/img/deleting.gif" width="450px" title="deleting" alt="npkill deleting">
</p>

<details>
<summary><em style="font-size:18px">More Examples</em></summary>
<p>
<ui>
<li>Search node_modules directories in your projects directory</li>
<code>$ npkill -d ~/projects</code></br></br>
<li>Displays the magenta color cursor... because I like magenta!</li>
<code>$ npkill --color magenta</code></br></br>
<li>List directories called "dist" and and show errors if any occur:</li>
<code>$ npkill --target dist -e</code></br></br>
<li>List vendor directories in your projects directory, sort by size, and show that in gb:</li>
<code>$ npkill -d '~/more projects' -gb --sort size --target vendor</code>
</ul>
</p>
</details>

</br></br>
